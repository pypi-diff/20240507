# Comparing `tmp/whatsapp_chat_analyze-0.1.3.tar.gz` & `tmp/whatsapp_chat_analyze-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp_chat_analyze-0.1.3.tar", max compression
+gzip compressed data, was "whatsapp_chat_analyze-0.1.4.tar", max compression
```

## Comparing `whatsapp_chat_analyze-0.1.3.tar` & `whatsapp_chat_analyze-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1682 2024-05-06 04:35:18.706328 whatsapp_chat_analyze-0.1.3/README.md
--rw-r--r--   0        0        0      898 2024-05-06 14:52:24.856626 whatsapp_chat_analyze-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-06 14:52:24.859608 whatsapp_chat_analyze-0.1.3/whatsapp_chat_analyze/__init__.py
--rwxr-xr-x   0        0        0    10916 2024-05-06 14:52:05.397668 whatsapp_chat_analyze-0.1.3/whatsapp_chat_analyze/cli.py
--rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 whatsapp_chat_analyze-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1682 2024-05-06 04:35:18.706328 whatsapp_chat_analyze-0.1.4/README.md
+-rw-r--r--   0        0        0      898 2024-05-07 02:58:37.488764 whatsapp_chat_analyze-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-07 02:58:37.489721 whatsapp_chat_analyze-0.1.4/whatsapp_chat_analyze/__init__.py
+-rwxr-xr-x   0        0        0    14106 2024-05-07 02:53:30.217582 whatsapp_chat_analyze-0.1.4/whatsapp_chat_analyze/cli.py
+-rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 whatsapp_chat_analyze-0.1.4/PKG-INFO
```

### Comparing `whatsapp_chat_analyze-0.1.3/README.md` & `whatsapp_chat_analyze-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `whatsapp_chat_analyze-0.1.3/pyproject.toml` & `whatsapp_chat_analyze-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whatsapp-chat-analyze"
-version = "0.1.3"
+version = "0.1.4"
 description = "Ingest and analyze WhatsApp chat data, and plot beautiful visualizations."
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/tddschn/whatsapp-chat-analyze"
 repository = "https://github.com/tddschn/whatsapp-chat-analyze"
 classifiers = ["Topic :: Utilities"]
```

### Comparing `whatsapp_chat_analyze-0.1.3/whatsapp_chat_analyze/cli.py` & `whatsapp_chat_analyze-0.1.4/whatsapp_chat_analyze/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -238,14 +238,100 @@
     )
 
     # save html
     fig.write_html(f"{output_base_name}-messages-per-day-by-author.html")
     print(f'Plot saved as "{output_base_name}-messages-per-day-by-author.html"')
 
 
+def plot_by_date_total_char_count(
+    df, output_base_name: str, chat_name: str | None = None
+):
+    print(
+        f'Plotting "Total Character Count per Day" and "Total Character Count per Day by Author"'
+    )
+    title_suffix = " | Made by Teddy (teddysc.me)"
+    title_prefix = f"{chat_name} |" if chat_name else ""
+    import plotly.express as px
+    import pandas as pd
+
+    # Ensure the 'Date' column is in datetime format
+    df["Date"] = pd.to_datetime(df["Date"])
+
+    # Calculate total characters for each message
+    df["TotalChars"] = df["Message"].apply(len)
+
+    # Generate a Series with the sum of characters per day
+    char_counts = df.groupby("Date")["TotalChars"].sum()
+
+    # Create a date range that covers all days from the minimum to the maximum date
+    all_dates = pd.date_range(
+        start=char_counts.index.min(), end=char_counts.index.max(), freq="D"
+    )
+
+    # Reindex the char_counts Series to include all dates in the range, filling missing values with 0
+    char_counts = char_counts.reindex(all_dates, fill_value=0)
+
+    # Create the Plotly figure using the adjusted character counts
+    fig = px.bar(
+        char_counts.reset_index(),
+        x="index",
+        y="TotalChars",
+        labels={"index": "Date", "TotalChars": "Total Characters"},
+        title=title_prefix + "Total Character Count per Day" + title_suffix,
+    )
+
+    # save html
+    fig.write_html(f"{output_base_name}-total-char-count-per-day.html")
+    print(f'Plot saved as "{output_base_name}-total-char-count-per-day.html"')
+
+    # Group by Date and Author, then sum characters
+    grouped_data = (
+        df.groupby(["Date", "Author"])["TotalChars"]
+        .sum()
+        .reset_index(name="TotalChars")
+    )
+
+    # Pivot the grouped_data DataFrame to get authors in columns, dates as index
+    pivot_data = grouped_data.pivot_table(
+        index="Date", columns="Author", values="TotalChars", fill_value=0
+    )
+
+    # Reindex the pivot table to include all dates in the range, filling missing values with 0
+    pivot_data = (
+        pivot_data.reindex(all_dates, fill_value=0).rename_axis("Date").reset_index()
+    )
+
+    # Melt the DataFrame back to a long form which is suitable for Plotly
+    melted_data = pivot_data.melt(
+        id_vars=["Date"], var_name="Author", value_name="TotalChars"
+    )
+
+    # Calculate total characters per day
+    total_chars_per_day = melted_data.groupby("Date")["TotalChars"].sum()
+
+    # Create a stacked bar chart
+    fig = px.bar(
+        melted_data,
+        x="Date",
+        y="TotalChars",
+        color="Author",
+        title=title_prefix + "Total Character Count per Day by Author" + title_suffix,
+        labels={"Date": "Date", "TotalChars": "Total Characters"},
+        text_auto=True,  # Automatically format text in bars
+        hover_data={
+            "TotalChars": True,  # Show number of characters in hover
+            "Date": True,  # Don't repeat the date in hover
+        },
+    )
+
+    # save html
+    fig.write_html(f"{output_base_name}-total-char-count-per-day-by-author.html")
+    print(f'Plot saved as "{output_base_name}-total-char-count-per-day-by-author.html"')
+
+
 def main():
     args = get_args()
     # surpress warnings
     import warnings
 
     warnings.filterwarnings("ignore")
 
@@ -268,42 +354,47 @@
                     raise ValueError(
                         f"Expected 1 .txt file in the zip, found {len(txt_files)}"
                     )
                 print(f'Analyzing "{args.file}"')
                 if args.extract_only:
                     return
 
-                import pandas as pd
-
-                data = parse_chat(args.file)
-                df = pd.DataFrame(data, columns=["Date", "Time", "Author", "Message"])
-                if args.to_csv_only:
-                    df.to_csv(args.file.with_suffix(".csv"), index=False)
-                    print(f'Chat saved as "{args.file.with_suffix(".csv")}"')
-                    return
-                if args.anonymize:
-                    # replace every name with a, b, ... z, aa, ab, ...
-                    import string
-
-                    authors = df["Author"].unique()
-                    author_map = dict(zip(authors, string.ascii_uppercase))
-                    df["Author"] = df["Author"].map(author_map)
             finally:
                 pass
 
+    if args.extract_only:
+        print("Input file is not a zip file, nothing to extract. Exiting.")
+        return
+    import pandas as pd
+
+    data = parse_chat(args.file)
+    df = pd.DataFrame(data, columns=["Date", "Time", "Author", "Message"])
+    if args.to_csv_only:
+        df.to_csv(args.file.with_suffix(".csv"), index=False)
+        print(f'Chat saved as "{args.file.with_suffix(".csv")}"')
+        return
+    if args.anonymize:
+        # replace every name with a, b, ... z, aa, ab, ...
+        import string
+
+        authors = df["Author"].unique()
+        author_map = dict(zip(authors, string.ascii_uppercase))
+        df["Author"] = df["Author"].map(author_map)
+
     # pcp_extra_args = {"plotly": args.plotly}
     pcp_extra_args = {"plotly": True}
     common_args = {}
     if args.chat_name:
         common_args["chat_name"] = args.chat_name
     if not args.by_day_only:
         plot_count_plots(
             df, args.output_base_name, "message_count", **common_args | pcp_extra_args
         )
         plot_count_plots(
             df, args.output_base_name, "char_count", **common_args | pcp_extra_args
         )
     plot_by_date(df, args.output_base_name, **common_args)
+    plot_by_date_total_char_count(df, args.output_base_name, **common_args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `whatsapp_chat_analyze-0.1.3/PKG-INFO` & `whatsapp_chat_analyze-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chat-analyze
-Version: 0.1.3
+Version: 0.1.4
 Summary: Ingest and analyze WhatsApp chat data, and plot beautiful visualizations.
 Home-page: https://github.com/tddschn/whatsapp-chat-analyze
 License: MIT
 Keywords: cli,utility,whatsapp,chat,analyze,visualization
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

