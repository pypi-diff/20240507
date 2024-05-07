# Comparing `tmp/vfs_appointment_bot-1.0.0.tar.gz` & `tmp/vfs_appointment_bot-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vfs_appointment_bot-1.0.0.tar", max compression
+gzip compressed data, was "vfs_appointment_bot-1.1.0.tar", max compression
```

## Comparing `vfs_appointment_bot-1.0.0.tar` & `vfs_appointment_bot-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1071 2024-04-27 09:23:31.960575 vfs_appointment_bot-1.0.0/LICENSE
--rw-r--r--   0        0        0    10862 2024-04-27 09:23:31.960575 vfs_appointment_bot-1.0.0/README.md
--rw-r--r--   0        0        0      972 2024-04-27 09:23:31.960575 vfs_appointment_bot-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3965 2024-04-27 09:23:31.960575 vfs_appointment_bot-1.0.0/vfs_appointment_bot/main.py
--rw-r--r--   0        0        0     1992 2024-04-27 09:23:31.960575 vfs_appointment_bot-1.0.0/vfs_appointment_bot/notification/email_client.py
--rw-r--r--   0        0        0     2717 2024-04-27 09:23:31.960575 vfs_appointment_bot-1.0.0/vfs_appointment_bot/notification/notification_client.py
--rw-r--r--   0        0        0     1385 2024-04-27 09:23:31.964576 vfs_appointment_bot-1.0.0/vfs_appointment_bot/notification/notification_client_factory.py
--rw-r--r--   0        0        0     1937 2024-04-27 09:23:31.964576 vfs_appointment_bot-1.0.0/vfs_appointment_bot/notification/telegram_client.py
--rw-r--r--   0        0        0     4279 2024-04-27 09:23:31.964576 vfs_appointment_bot-1.0.0/vfs_appointment_bot/notification/twilio_client.py
--rw-r--r--   0        0        0     1996 2024-04-27 09:23:31.964576 vfs_appointment_bot-1.0.0/vfs_appointment_bot/utils/config_reader.py
--rw-r--r--   0        0        0      231 2024-04-27 09:23:31.964576 vfs_appointment_bot-1.0.0/vfs_appointment_bot/utils/date_utils.py
--rw-r--r--   0        0        0      653 2024-04-27 09:23:31.964576 vfs_appointment_bot-1.0.0/vfs_appointment_bot/utils/timer.py
--rw-r--r--   0        0        0     8576 2024-04-27 09:23:31.964576 vfs_appointment_bot-1.0.0/vfs_appointment_bot/vfs_bot/vfs_bot.py
--rw-r--r--   0        0        0     5966 2024-04-27 09:23:31.964576 vfs_appointment_bot-1.0.0/vfs_appointment_bot/vfs_bot/vfs_bot_de.py
--rw-r--r--   0        0        0     1251 2024-04-27 09:23:31.964576 vfs_appointment_bot-1.0.0/vfs_appointment_bot/vfs_bot/vfs_bot_factory.py
--rw-r--r--   0        0        0    11910 1970-01-01 00:00:00.000000 vfs_appointment_bot-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-07 01:44:09.117003 vfs_appointment_bot-1.1.0/LICENSE
+-rw-r--r--   0        0        0    12410 2024-05-07 01:44:09.117003 vfs_appointment_bot-1.1.0/README.md
+-rw-r--r--   0        0        0      972 2024-05-07 01:44:09.117003 vfs_appointment_bot-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4030 2024-05-07 01:44:09.117003 vfs_appointment_bot-1.1.0/vfs_appointment_bot/main.py
+-rw-r--r--   0        0        0     1992 2024-05-07 01:44:09.117003 vfs_appointment_bot-1.1.0/vfs_appointment_bot/notification/email_client.py
+-rw-r--r--   0        0        0     2717 2024-05-07 01:44:09.117003 vfs_appointment_bot-1.1.0/vfs_appointment_bot/notification/notification_client.py
+-rw-r--r--   0        0        0     1385 2024-05-07 01:44:09.121003 vfs_appointment_bot-1.1.0/vfs_appointment_bot/notification/notification_client_factory.py
+-rw-r--r--   0        0        0     1937 2024-05-07 01:44:09.121003 vfs_appointment_bot-1.1.0/vfs_appointment_bot/notification/telegram_client.py
+-rw-r--r--   0        0        0     4279 2024-05-07 01:44:09.121003 vfs_appointment_bot-1.1.0/vfs_appointment_bot/notification/twilio_client.py
+-rw-r--r--   0        0        0     2087 2024-05-07 01:44:09.121003 vfs_appointment_bot-1.1.0/vfs_appointment_bot/utils/config_reader.py
+-rw-r--r--   0        0        0      231 2024-05-07 01:44:09.121003 vfs_appointment_bot-1.1.0/vfs_appointment_bot/utils/date_utils.py
+-rw-r--r--   0        0        0      658 2024-05-07 01:44:09.121003 vfs_appointment_bot-1.1.0/vfs_appointment_bot/utils/timer.py
+-rw-r--r--   0        0        0     8711 2024-05-07 01:44:09.121003 vfs_appointment_bot-1.1.0/vfs_appointment_bot/vfs_bot/vfs_bot.py
+-rw-r--r--   0        0        0     5966 2024-05-07 01:44:09.121003 vfs_appointment_bot-1.1.0/vfs_appointment_bot/vfs_bot/vfs_bot_de.py
+-rw-r--r--   0        0        0     1362 2024-05-07 01:44:09.121003 vfs_appointment_bot-1.1.0/vfs_appointment_bot/vfs_bot/vfs_bot_factory.py
+-rw-r--r--   0        0        0     6478 2024-05-07 01:44:09.121003 vfs_appointment_bot-1.1.0/vfs_appointment_bot/vfs_bot/vfs_bot_it.py
+-rw-r--r--   0        0        0    13458 1970-01-01 00:00:00.000000 vfs_appointment_bot-1.1.0/PKG-INFO
```

### Comparing `vfs_appointment_bot-1.0.0/LICENSE` & `vfs_appointment_bot-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vfs_appointment_bot-1.0.0/README.md` & `vfs_appointment_bot-1.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,133 @@
 # VFS Appointment Bot
 
 [![GitHub License](https://img.shields.io/github/license/ranjan-mohanty/vfs-appointment-bot)](https://github.com/ranjan-mohanty/vfs-appointment-bot/blob/main/LICENSE)
+[![GitHub Release](https://img.shields.io/github/v/release/ranjan-mohanty/vfs-appointment-bot?logo=GitHub)](https://github.com/ranjan-mohanty/vfs-appointment-bot/releases)
+[![PyPI - Version](https://img.shields.io/pypi/v/vfs-appointment-bot?logo=pypi)](https://pypi.org/project/vfs-appointment-bot)
+[![Downloads](https://static.pepy.tech/badge/vfs-appointment-bot)](https://pepy.tech/project/vfs-appointment-bot)
+[![Endpoint Badge](https://img.shields.io/endpoint?url=https%3A%2F%2Fhits.dwyl.com%2Franjan-mohanty%2Fvfs-appointment-bot.json&style=flat&logo=GitHub&label=views)](https://github.com/ranjan-mohanty/vfs-appointment-bot)
 [![GitHub forks](https://img.shields.io/github/forks/ranjan-mohanty/vfs-appointment-bot)](https://github.com/ranjan-mohanty/vfs-appointment-bot/forks)
 [![GitHub Repo stars](https://img.shields.io/github/stars/ranjan-mohanty/vfs-appointment-bot)](https://github.com/ranjan-mohanty/vfs-appointment-bot/stargazers)
 
-<!-- [![GitHub Release](https://img.shields.io/github/v/release/ranjan-mohanty/vfs-appointment-bot)](https://github.com/ranjan-mohanty/vfs-appointment-bot/releases)
-[![PyPI - Version](https://img.shields.io/pypi/v/vfs-appointment-bot)](https://pypi.org/project/vfs-appointment-bot/)
-[![Downloads](https://static.pepy.tech/badge/vfs-appointment-bot)](https://pepy.tech/project/vfs-appointment-bot) -->
-
 [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/ranjan-mohanty/vfs-appointment-bot/build.yml)](https://github.com/ranjan-mohanty/vfs-appointment-bot/actions/workflows/build.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/21f1ecd428ec4342980020a6ef383439)](https://app.codacy.com/gh/ranjan-mohanty/vfs-appointment-bot/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/ranjan-mohanty/vfs-appointment-bot/badge)](https://securityscorecards.dev/viewer/?uri=github.com/ranjan-mohanty/vfs-appointment-bot)
 [![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/ranjan-mohanty/vfs-appointment-bot)](https://github.com/ranjan-mohanty/vfs-appointment-bot/issues)
 ![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/ranjan-mohanty/vfs-appointment-bot)
 [![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Franjan-mohanty%2Fvfs-appointment-bot)](https://twitter.com/intent/tweet?text=Check%20this%20out%20&url=https%3A%2F%2Fgithub.com%2Franjan-mohanty%2Fvfs-appointment-bot)
 
 This Python script(**vfs-appointment-bot**) automates checking for appointments at VFS Global portal in a specified country.
 
 ## Installation
 
-<!-- The `vfs-appointment-bot` script can be installed using two methods:
+The `vfs-appointment-bot` script can be installed using two methods:
 
-**1. Using pip:**
+### 1. Using pip
 
 It is the preferred method for installing `vfs-appointment-bot`. Here's how to do it:
 
-1.  **Install using pip:**
+1. **Create a virtual environment (Recommended):**
 
-    ```bash
-    pip install vfs-appointment-bot
-    ```
+   ```bash
+   python3 -m venv venv
+   ```
 
-    This will download and install the `vfs-appointment-bot` package and its dependencies into your Python environment.
+   This creates a virtual environment named `venv` to isolate project dependencies from your system-wide Python installation (**recommended**).
 
-**Manual Installation:**
+2. **Activate the virtual environment:**
 
-If you prefer a more traditional approach, you can clone the source code from the project repository and install it manually: -->
+   **Linux/macOS:**
 
-1.  **Clone the repository:**
+   ```bash
+   source venv/bin/activate
+   ```
 
-    ```bash
-    git clone https://github.com/ranjan-mohanty/vfs-appointment-bot
-    ```
+   **Windows:**
 
-2.  **Navigate to the project directory:**
+   ```bash
+   venv\Scripts\activate
+   ```
 
-    ```bash
-    cd vfs-appointment-bot
-    ```
+3. **Install using pip:**
 
-3.  **Create a virtual environment (Recommended):**
+   ```bash
+   pip install vfs-appointment-bot
+   ```
 
-    ```bash
-    python3 -m venv venv
-    ```
+   This will download and install the `vfs-appointment-bot` package and its dependencies into your Python environment.
 
-    This creates a virtual environment named `venv` to isolate project dependencies from your system-wide Python installation (**recommended**).
+### 2. Manual Installation
 
-4.  **Activate the virtual environment:**
+For an alternative installation method, clone the source code from the project repository and install it manually.
 
-    **Linux/macOS:**
+1. **Clone the repository:**
 
-    ```bash
-    source venv/bin/activate
-    ```
+   ```bash
+   git clone https://github.com/ranjan-mohanty/vfs-appointment-bot
+   ```
 
-    **Windows:**
+2. **Navigate to the project directory:**
 
-    ```bash
-    venv\Scripts\activate
-    ```
+   ```bash
+   cd vfs-appointment-bot
+   ```
 
-5.  **Install dependencies:**
+3. **Create a virtual environment (Recommended):**
 
-    ```bash
-    pip install poetry
-    poetry install
-    ```
+   ```bash
+   python3 -m venv venv
+   ```
 
-6.  **Install playwright dependencies:**
+   This creates a virtual environment named `venv` to isolate project dependencies from your system-wide Python installation (**recommended**).
 
-    ```bash
-    playwright install
-    ```
+4. **Activate the virtual environment:**
 
-## Usage
+   **Linux/macOS:**
+
+   ```bash
+   source venv/bin/activate
+   ```
+
+   **Windows:**
+
+   ```bash
+   venv\Scripts\activate
+   ```
+
+5. **Install dependencies:**
+
+   ```bash
+   pip install poetry
+   poetry install
+   ```
+
+6. **Install playwright dependencies:**
+
+   ```bash
+   playwright install
+   ```
 
-> **Pre-configuration:**  
-> Before running the script, ensure your update the vfs credentials and notification channel preferences in the config.ini file. See the [Notification Channels](#notification-channels) section for details on configuring email, Twilio, and Telegram notifications.
+## Configuration
+
+1. Download the [`config/config.ini`](https://raw.githubusercontent.com/ranjan-mohanty/vfs-appointment-bot/main/config/config.ini) template.
+
+   ```bash
+   curl -L https://raw.githubusercontent.com/ranjan-mohanty/vfs-appointment-bot/main/config/config.ini -o config.ini
+   ```
+
+2. Update the vfs credentials and notification channel preferences. See the [Notification Channels](#notification-channels) section for details on configuring email, Twilio, and Telegram notifications.
+3. Export the path of the config file to the environment variable `VFS_BOT_CONFIG_PATH`
+
+   ```bash
+   export VFS_BOT_CONFIG_PATH=<your-config-path>/config.ini
+   ```
+
+**If you installed the script by cloning the repository (manual installation)**, you can directly edit the values in `config/config.ini`.
+
+## Usage
 
 1. **Command-Line Argument:**
 
    The script requires the source and destination country code ([as per ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2#Officially_assigned_code_elements)) to be provided as a command-line argument using the `-sc` or `--source-country-code` and `-dc` or `--destination-country-code` option.
 
 2. **Running the Script:**
 
@@ -156,18 +192,20 @@
    - **`bot_token` (Required):** Your Telegram bot token obtained from BotFather.
    - **`chat_id` (Optional):** The specific Telegram chat ID where you want to receive notifications. If omitted, the bot will send notifications to the chat where it was messaged from. To find your chat ID, you can create a group chat with just yourself and then use the `/my_id` command within the bot.
 
 ## Supported Countries and Appointment Parameters
 
 The following table lists currently supported countries and their corresponding appointment parameters:
 
-| Country                 | Appointment Parameters                        |
-| ----------------------- | --------------------------------------------- |
-| India(IN) - Germany(DE) | visa_category, visa_sub_category, visa_center |
-| Iraq(IQ) - Germany(DE)  | visa_category, visa_sub_category, visa_center |
+| Country                    | Appointment Parameters                                      |
+| -------------------------- | ----------------------------------------------------------- |
+| India(IN) - Germany(DE)    | visa_category, visa_sub_category, visa_center               |
+| Iraq(IQ) - Germany(DE)     | visa_category, visa_sub_category, visa_center               |
+| Morocco(MA) - Italy(IT)    | visa_category, visa_sub_category, visa_center, payment_mode |
+| Azerbaijan(AZ) - Italy(IT) | visa_category, visa_sub_category, visa_center               |
 
 **Notes:**
 
 - Appointment parameters might vary depending on the specific country and visa type. Always consult VFS Global's website for the latest information.
 
 ## Known Issues
 
@@ -195,10 +233,14 @@
 
 We welcome contributions from the community to improve this project! Here's how you can get involved:
 
 - **Report issues:** If you encounter any bugs or problems with the script, please create an issue on the project's repository.
 - **Suggest improvements:** Do you have ideas for making the script more user-friendly or feature-rich? Feel free to create an issue or pull request on the repository.
 - **Submit pull requests:** If you've made code changes that you think would benefit the project, create a pull request on the repository. Please follow any contribution guidelines outlined in a CONTRIBUTING.md file.
 
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=ranjan-mohanty/vfs-appointment-bot&type=Date)](https://star-history.com/#ranjan-mohanty/vfs-appointment-bot&Date)
+
 ## Disclaimer
 
 This script is provided as-is and is not affiliated with VFS Global. It's your responsibility to ensure you're complying with VFS Global's terms and conditions when using this script. Be aware that website structures and appointment availability mechanisms might change over time.
```

### Comparing `vfs_appointment_bot-1.0.0/pyproject.toml` & `vfs_appointment_bot-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Project metadata
 [tool.poetry]
 name = "vfs-appointment-bot"
-version = "1.0.0"
+version = "1.1.0"
 description = "VFS Appointment Bot - This script automates checking for appointments at VFS Global offices in a specified country."
 authors = ["Ranjan Mohanty <ranjan@duck.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["vfs", "vfs-bot", "vfs-appointment-bot", "visa-appointment-bot"]
 
 # URLs
```

### Comparing `vfs_appointment_bot-1.0.0/vfs_appointment_bot/main.py` & `vfs_appointment_bot-1.1.0/vfs_appointment_bot/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import logging
 import sys
 from typing import Dict
 
-from vfs_appointment_bot.utils.config_reader import get_config_value
+from vfs_appointment_bot.utils.config_reader import get_config_value, initialize_config
 from vfs_appointment_bot.utils.timer import countdown
 from vfs_appointment_bot.vfs_bot.vfs_bot import LoginError
 from vfs_appointment_bot.vfs_bot.vfs_bot_factory import (
     UnsupportedCountryError,
     get_vfs_bot,
 )
 
@@ -42,14 +42,15 @@
     unexpected errors, logging them appropriately.
 
     Raises:
         UnsupportedCountryError: If the provided country code is not supported by the bot.
         Exception: For any other unexpected errors encountered during execution.
     """
     initialize_logger()
+    initialize_config()
 
     parser = argparse.ArgumentParser(
         description="VFS Appointment Bot: Checks for appointments at VFS Global"
     )
     required_args = parser.add_argument_group("required arguments")
     required_args.add_argument(
         "-sc",
@@ -85,15 +86,16 @@
     try:
         while True:
             vfs_bot = get_vfs_bot(source_country_code, destination_country_code)
             appointment_found = vfs_bot.run(args)
             if appointment_found:
                 break
             countdown(
-                get_config_value("default", "interval"), "Next appointment check in"
+                int(get_config_value("default", "interval")),
+                "Next appointment check in",
             )
 
     except (UnsupportedCountryError, LoginError) as e:
         logging.error(e)
     except Exception as e:
         logging.exception(e)
```

### Comparing `vfs_appointment_bot-1.0.0/vfs_appointment_bot/notification/email_client.py` & `vfs_appointment_bot-1.1.0/vfs_appointment_bot/notification/email_client.py`

 * *Files identical despite different names*

### Comparing `vfs_appointment_bot-1.0.0/vfs_appointment_bot/notification/notification_client.py` & `vfs_appointment_bot-1.1.0/vfs_appointment_bot/notification/notification_client.py`

 * *Files identical despite different names*

### Comparing `vfs_appointment_bot-1.0.0/vfs_appointment_bot/notification/notification_client_factory.py` & `vfs_appointment_bot-1.1.0/vfs_appointment_bot/notification/notification_client_factory.py`

 * *Files identical despite different names*

### Comparing `vfs_appointment_bot-1.0.0/vfs_appointment_bot/notification/telegram_client.py` & `vfs_appointment_bot-1.1.0/vfs_appointment_bot/notification/telegram_client.py`

 * *Files identical despite different names*

### Comparing `vfs_appointment_bot-1.0.0/vfs_appointment_bot/notification/twilio_client.py` & `vfs_appointment_bot-1.1.0/vfs_appointment_bot/notification/twilio_client.py`

 * *Files identical despite different names*

### Comparing `vfs_appointment_bot-1.0.0/vfs_appointment_bot/utils/config_reader.py` & `vfs_appointment_bot-1.1.0/vfs_appointment_bot/utils/config_reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 import os
 from configparser import ConfigParser
 from typing import Dict
 
-_config = None
+_config: ConfigParser = None
 
 
-def get_config_parser(config_dir="config"):
+def initialize_config(config_dir="config"):
     """
     Reads all INI configuration files in a directory and caches the result.
+    Also reads user config from `VFS_BOT_CONFIG_PATH` env var (if set)
 
     Args:
         config_dir: The directory containing configuration files (default: "config").
-
-    Returns:
-        A ConfigParser object loaded with configuration data.
     """
     global _config
     if not _config:
         _config = ConfigParser()
         for entry in os.scandir(config_dir):
             if entry.is_file() and entry.name.endswith(".ini"):
                 config_file_path = os.path.join(config_dir, entry.name)
                 _config.read(config_file_path)
-    return _config
+
+    # Read user defined config file
+    user_config_path = os.environ.get("VFS_BOT_CONFIG_PATH")
+    if user_config_path:
+        _config.read(user_config_path)
 
 
 def get_config_section(section: str, default: Dict = None) -> Dict:
     """
     Get a configuration section as a dictionary.
 
     Args:
         section: The name of the section to retrieve.
         default: A dictionary containing default values for the section (optional).
 
     Returns:
         A dictionary containing the configuration for the specified section,
         or the provided default dictionary if the section is not found.
     """
-    config = get_config_parser()
-    if config.has_section(section):
-        return dict(config[section])
+    if _config.has_section(section):
+        return dict(_config[section])
     else:
         return default or {}
 
 
 def get_config_value(section: str, key: str, default: str = None) -> str:
     """
     Get a specific configuration value.
@@ -53,12 +54,11 @@
         key: The name of the key to retrieve.
         default: The default value to return if the section or key is not found (optional).
 
     Returns:
         The value associated with the given key within the specified section,
         or the provided default value if the section or key does not exist.
     """
-    config = get_config_parser()
-    if config.has_section(section) and config.has_option(section, key):
-        return config[section][key]
+    if _config.has_section(section) and _config.has_option(section, key):
+        return _config[section][key]
     else:
         return default
```

### Comparing `vfs_appointment_bot-1.0.0/vfs_appointment_bot/utils/timer.py` & `vfs_appointment_bot-1.1.0/vfs_appointment_bot/utils/timer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 
 from tqdm import tqdm
 
 
-def countdown(t, message="Countdown", unit="seconds"):
+def countdown(t: int, message="Countdown", unit="seconds"):
     """
     Implements a countdown timer
 
     Args:
         t (int): The initial countdown time in the specified unit (e.g., seconds, minutes).
         message (str, optional): The message to display during the countdown.
                                 Defaults to "Countdown".
```

### Comparing `vfs_appointment_bot-1.0.0/vfs_appointment_bot/vfs_bot/vfs_bot.py` & `vfs_appointment_bot-1.1.0/vfs_appointment_bot/vfs_bot/vfs_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,28 +53,31 @@
         logging.info(
             f"Starting VFS Bot for {self.source_country_code.upper()}-{self.destination_country_code.upper()}"
         )
 
         # Configuration values
         try:
             browser_type = get_config_value("browser", "type", "firefox")
+            headless_mode = get_config_value("browser", "headless", "True")
             url_key = self.source_country_code + "-" + self.destination_country_code
             vfs_url = get_config_value("vfs-url", url_key)
         except KeyError as e:
             logging.error(f"Missing configuration value: {e}")
             return
 
         email_id = get_config_value("vfs-credential", "email")
         password = get_config_value("vfs-credential", "password")
 
         appointment_params = self.get_appointment_params(args)
 
         # Launch browser and perform actions
         with sync_playwright() as p:
-            browser = getattr(p, browser_type).launch(headless=True)
+            browser = getattr(p, browser_type).launch(
+                headless=headless_mode in ("True", "true")
+            )
             page = browser.new_page()
             stealth_sync(page)
 
             page.goto(vfs_url)
             self.pre_login_steps(page)
 
             try:
```

### Comparing `vfs_appointment_bot-1.0.0/vfs_appointment_bot/vfs_bot/vfs_bot_de.py` & `vfs_appointment_bot-1.1.0/vfs_appointment_bot/vfs_bot/vfs_bot_de.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         to the destination country's VFS website.
 
         Args:
             source_country_code (str): The country code where you're applying from.
         """
         super().__init__()
         self.source_country_code = source_country_code
-        self.destination_country_code = "de"
+        self.destination_country_code = "DE"
         self.appointment_param_keys = [
             "visa_center",
             "visa_category",
             "visa_sub_category",
         ]
 
     def login(self, page: Page, email_id: str, password: str) -> None:
```

### Comparing `vfs_appointment_bot-1.0.0/vfs_appointment_bot/vfs_bot/vfs_bot_factory.py` & `vfs_appointment_bot-1.1.0/vfs_appointment_bot/vfs_bot/vfs_bot_factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,17 +19,21 @@
     Returns:
         VfsBot: An instance of the `VfsBot` subclass specific to the provided country.
 
     Raises:
         UnsupportedCountryError: If the provided country is not supported.
     """
 
-    country_lower = destination_country_code.lower()
+    country_lower = destination_country_code
 
-    if country_lower == "de":
+    if country_lower == "DE":
         from .vfs_bot_de import VfsBotDe
 
         return VfsBotDe(source_country_code)
+    elif country_lower == "IT":
+        from .vfs_bot_it import VfsBotIt
+
+        return VfsBotIt(source_country_code)
     else:
         raise UnsupportedCountryError(
             f"Country {destination_country_code} is not supported"
         )
```

### Comparing `vfs_appointment_bot-1.0.0/PKG-INFO` & `vfs_appointment_bot-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vfs-appointment-bot
-Version: 1.0.0
+Version: 1.1.0
 Summary: VFS Appointment Bot - This script automates checking for appointments at VFS Global offices in a specified country.
 License: MIT
 Keywords: vfs,vfs-bot,vfs-appointment-bot,visa-appointment-bot
 Author: Ranjan Mohanty
 Author-email: ranjan@duck.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,101 +20,137 @@
 Project-URL: homepage, https://github.com/ranjan-mohanty/vfs-appointment-bot/blob/main
 Project-URL: repository, https://github.com/ranjan-mohanty/vfs-appointment-bot/blob/main/README.md
 Description-Content-Type: text/markdown
 
 # VFS Appointment Bot
 
 [![GitHub License](https://img.shields.io/github/license/ranjan-mohanty/vfs-appointment-bot)](https://github.com/ranjan-mohanty/vfs-appointment-bot/blob/main/LICENSE)
+[![GitHub Release](https://img.shields.io/github/v/release/ranjan-mohanty/vfs-appointment-bot?logo=GitHub)](https://github.com/ranjan-mohanty/vfs-appointment-bot/releases)
+[![PyPI - Version](https://img.shields.io/pypi/v/vfs-appointment-bot?logo=pypi)](https://pypi.org/project/vfs-appointment-bot)
+[![Downloads](https://static.pepy.tech/badge/vfs-appointment-bot)](https://pepy.tech/project/vfs-appointment-bot)
+[![Endpoint Badge](https://img.shields.io/endpoint?url=https%3A%2F%2Fhits.dwyl.com%2Franjan-mohanty%2Fvfs-appointment-bot.json&style=flat&logo=GitHub&label=views)](https://github.com/ranjan-mohanty/vfs-appointment-bot)
 [![GitHub forks](https://img.shields.io/github/forks/ranjan-mohanty/vfs-appointment-bot)](https://github.com/ranjan-mohanty/vfs-appointment-bot/forks)
 [![GitHub Repo stars](https://img.shields.io/github/stars/ranjan-mohanty/vfs-appointment-bot)](https://github.com/ranjan-mohanty/vfs-appointment-bot/stargazers)
 
-<!-- [![GitHub Release](https://img.shields.io/github/v/release/ranjan-mohanty/vfs-appointment-bot)](https://github.com/ranjan-mohanty/vfs-appointment-bot/releases)
-[![PyPI - Version](https://img.shields.io/pypi/v/vfs-appointment-bot)](https://pypi.org/project/vfs-appointment-bot/)
-[![Downloads](https://static.pepy.tech/badge/vfs-appointment-bot)](https://pepy.tech/project/vfs-appointment-bot) -->
-
 [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/ranjan-mohanty/vfs-appointment-bot/build.yml)](https://github.com/ranjan-mohanty/vfs-appointment-bot/actions/workflows/build.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/21f1ecd428ec4342980020a6ef383439)](https://app.codacy.com/gh/ranjan-mohanty/vfs-appointment-bot/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/ranjan-mohanty/vfs-appointment-bot/badge)](https://securityscorecards.dev/viewer/?uri=github.com/ranjan-mohanty/vfs-appointment-bot)
 [![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/ranjan-mohanty/vfs-appointment-bot)](https://github.com/ranjan-mohanty/vfs-appointment-bot/issues)
 ![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/ranjan-mohanty/vfs-appointment-bot)
 [![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Franjan-mohanty%2Fvfs-appointment-bot)](https://twitter.com/intent/tweet?text=Check%20this%20out%20&url=https%3A%2F%2Fgithub.com%2Franjan-mohanty%2Fvfs-appointment-bot)
 
 This Python script(**vfs-appointment-bot**) automates checking for appointments at VFS Global portal in a specified country.
 
 ## Installation
 
-<!-- The `vfs-appointment-bot` script can be installed using two methods:
+The `vfs-appointment-bot` script can be installed using two methods:
 
-**1. Using pip:**
+### 1. Using pip
 
 It is the preferred method for installing `vfs-appointment-bot`. Here's how to do it:
 
-1.  **Install using pip:**
+1. **Create a virtual environment (Recommended):**
 
-    ```bash
-    pip install vfs-appointment-bot
-    ```
+   ```bash
+   python3 -m venv venv
+   ```
 
-    This will download and install the `vfs-appointment-bot` package and its dependencies into your Python environment.
+   This creates a virtual environment named `venv` to isolate project dependencies from your system-wide Python installation (**recommended**).
 
-**Manual Installation:**
+2. **Activate the virtual environment:**
 
-If you prefer a more traditional approach, you can clone the source code from the project repository and install it manually: -->
+   **Linux/macOS:**
 
-1.  **Clone the repository:**
+   ```bash
+   source venv/bin/activate
+   ```
 
-    ```bash
-    git clone https://github.com/ranjan-mohanty/vfs-appointment-bot
-    ```
+   **Windows:**
 
-2.  **Navigate to the project directory:**
+   ```bash
+   venv\Scripts\activate
+   ```
 
-    ```bash
-    cd vfs-appointment-bot
-    ```
+3. **Install using pip:**
 
-3.  **Create a virtual environment (Recommended):**
+   ```bash
+   pip install vfs-appointment-bot
+   ```
 
-    ```bash
-    python3 -m venv venv
-    ```
+   This will download and install the `vfs-appointment-bot` package and its dependencies into your Python environment.
 
-    This creates a virtual environment named `venv` to isolate project dependencies from your system-wide Python installation (**recommended**).
+### 2. Manual Installation
 
-4.  **Activate the virtual environment:**
+For an alternative installation method, clone the source code from the project repository and install it manually.
 
-    **Linux/macOS:**
+1. **Clone the repository:**
 
-    ```bash
-    source venv/bin/activate
-    ```
+   ```bash
+   git clone https://github.com/ranjan-mohanty/vfs-appointment-bot
+   ```
 
-    **Windows:**
+2. **Navigate to the project directory:**
 
-    ```bash
-    venv\Scripts\activate
-    ```
+   ```bash
+   cd vfs-appointment-bot
+   ```
 
-5.  **Install dependencies:**
+3. **Create a virtual environment (Recommended):**
 
-    ```bash
-    pip install poetry
-    poetry install
-    ```
+   ```bash
+   python3 -m venv venv
+   ```
 
-6.  **Install playwright dependencies:**
+   This creates a virtual environment named `venv` to isolate project dependencies from your system-wide Python installation (**recommended**).
 
-    ```bash
-    playwright install
-    ```
+4. **Activate the virtual environment:**
 
-## Usage
+   **Linux/macOS:**
+
+   ```bash
+   source venv/bin/activate
+   ```
+
+   **Windows:**
+
+   ```bash
+   venv\Scripts\activate
+   ```
+
+5. **Install dependencies:**
+
+   ```bash
+   pip install poetry
+   poetry install
+   ```
+
+6. **Install playwright dependencies:**
+
+   ```bash
+   playwright install
+   ```
 
-> **Pre-configuration:**  
-> Before running the script, ensure your update the vfs credentials and notification channel preferences in the config.ini file. See the [Notification Channels](#notification-channels) section for details on configuring email, Twilio, and Telegram notifications.
+## Configuration
+
+1. Download the [`config/config.ini`](https://raw.githubusercontent.com/ranjan-mohanty/vfs-appointment-bot/main/config/config.ini) template.
+
+   ```bash
+   curl -L https://raw.githubusercontent.com/ranjan-mohanty/vfs-appointment-bot/main/config/config.ini -o config.ini
+   ```
+
+2. Update the vfs credentials and notification channel preferences. See the [Notification Channels](#notification-channels) section for details on configuring email, Twilio, and Telegram notifications.
+3. Export the path of the config file to the environment variable `VFS_BOT_CONFIG_PATH`
+
+   ```bash
+   export VFS_BOT_CONFIG_PATH=<your-config-path>/config.ini
+   ```
+
+**If you installed the script by cloning the repository (manual installation)**, you can directly edit the values in `config/config.ini`.
+
+## Usage
 
 1. **Command-Line Argument:**
 
    The script requires the source and destination country code ([as per ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2#Officially_assigned_code_elements)) to be provided as a command-line argument using the `-sc` or `--source-country-code` and `-dc` or `--destination-country-code` option.
 
 2. **Running the Script:**
 
@@ -179,18 +215,20 @@
    - **`bot_token` (Required):** Your Telegram bot token obtained from BotFather.
    - **`chat_id` (Optional):** The specific Telegram chat ID where you want to receive notifications. If omitted, the bot will send notifications to the chat where it was messaged from. To find your chat ID, you can create a group chat with just yourself and then use the `/my_id` command within the bot.
 
 ## Supported Countries and Appointment Parameters
 
 The following table lists currently supported countries and their corresponding appointment parameters:
 
-| Country                 | Appointment Parameters                        |
-| ----------------------- | --------------------------------------------- |
-| India(IN) - Germany(DE) | visa_category, visa_sub_category, visa_center |
-| Iraq(IQ) - Germany(DE)  | visa_category, visa_sub_category, visa_center |
+| Country                    | Appointment Parameters                                      |
+| -------------------------- | ----------------------------------------------------------- |
+| India(IN) - Germany(DE)    | visa_category, visa_sub_category, visa_center               |
+| Iraq(IQ) - Germany(DE)     | visa_category, visa_sub_category, visa_center               |
+| Morocco(MA) - Italy(IT)    | visa_category, visa_sub_category, visa_center, payment_mode |
+| Azerbaijan(AZ) - Italy(IT) | visa_category, visa_sub_category, visa_center               |
 
 **Notes:**
 
 - Appointment parameters might vary depending on the specific country and visa type. Always consult VFS Global's website for the latest information.
 
 ## Known Issues
 
@@ -218,11 +256,15 @@
 
 We welcome contributions from the community to improve this project! Here's how you can get involved:
 
 - **Report issues:** If you encounter any bugs or problems with the script, please create an issue on the project's repository.
 - **Suggest improvements:** Do you have ideas for making the script more user-friendly or feature-rich? Feel free to create an issue or pull request on the repository.
 - **Submit pull requests:** If you've made code changes that you think would benefit the project, create a pull request on the repository. Please follow any contribution guidelines outlined in a CONTRIBUTING.md file.
 
+## Star History
+
+[![Star History Chart](https://api.star-history.com/svg?repos=ranjan-mohanty/vfs-appointment-bot&type=Date)](https://star-history.com/#ranjan-mohanty/vfs-appointment-bot&Date)
+
 ## Disclaimer
 
 This script is provided as-is and is not affiliated with VFS Global. It's your responsibility to ensure you're complying with VFS Global's terms and conditions when using this script. Be aware that website structures and appointment availability mechanisms might change over time.
```

