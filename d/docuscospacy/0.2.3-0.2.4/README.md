# Comparing `tmp/docuscospacy-0.2.3.tar.gz` & `tmp/docuscospacy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docuscospacy-0.2.3.tar", last modified: Fri Oct  7 17:24:55 2022, max compression
+gzip compressed data, was "docuscospacy-0.2.4.tar", last modified: Tue May  7 18:33:56 2024, max compression
```

## Comparing `docuscospacy-0.2.3.tar` & `docuscospacy-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 user       (502) staff       (20)        0 2022-10-07 17:24:55.019984 docuscospacy-0.2.3/
--rw-r--r--   0 user       (502) staff       (20)    11357 2022-09-02 12:07:47.000000 docuscospacy-0.2.3/LICENSE
--rw-r--r--   0 user       (502) staff       (20)     4704 2022-10-07 17:24:55.019727 docuscospacy-0.2.3/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)     4358 2022-09-02 12:07:47.000000 docuscospacy-0.2.3/README.rst
-drwxr-xr-x   0 user       (502) staff       (20)        0 2022-10-07 17:24:55.015465 docuscospacy-0.2.3/docuscospacy/
--rw-r--r--   0 user       (502) staff       (20)        0 2022-09-02 12:07:47.000000 docuscospacy-0.2.3/docuscospacy/__init__.py
--rw-r--r--   0 user       (502) staff       (20)    18256 2022-10-07 17:18:32.000000 docuscospacy-0.2.3/docuscospacy/corpus_analysis.py
--rw-r--r--   0 user       (502) staff       (20)    44585 2022-09-02 21:05:50.000000 docuscospacy-0.2.3/docuscospacy/corpus_utils.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2022-10-07 17:24:55.019335 docuscospacy-0.2.3/docuscospacy.egg-info/
--rw-r--r--   0 user       (502) staff       (20)     4704 2022-10-07 17:24:54.000000 docuscospacy-0.2.3/docuscospacy.egg-info/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)      292 2022-10-07 17:24:54.000000 docuscospacy-0.2.3/docuscospacy.egg-info/SOURCES.txt
--rw-r--r--   0 user       (502) staff       (20)        1 2022-10-07 17:24:54.000000 docuscospacy-0.2.3/docuscospacy.egg-info/dependency_links.txt
--rw-r--r--   0 user       (502) staff       (20)       86 2022-10-07 17:24:54.000000 docuscospacy-0.2.3/docuscospacy.egg-info/requires.txt
--rw-r--r--   0 user       (502) staff       (20)       13 2022-10-07 17:24:54.000000 docuscospacy-0.2.3/docuscospacy.egg-info/top_level.txt
--rw-r--r--   0 user       (502) staff       (20)       38 2022-10-07 17:24:55.020116 docuscospacy-0.2.3/setup.cfg
--rw-r--r--   0 user       (502) staff       (20)      961 2022-10-07 17:21:05.000000 docuscospacy-0.2.3/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-07 18:33:56.666578 docuscospacy-0.2.4/
+-rw-r--r--   0 user       (501) staff       (20)    11357 2023-01-16 17:48:32.000000 docuscospacy-0.2.4/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     4685 2024-05-07 18:33:56.666040 docuscospacy-0.2.4/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     4358 2023-01-16 17:48:32.000000 docuscospacy-0.2.4/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-07 18:33:56.662974 docuscospacy-0.2.4/docuscospacy/
+-rw-r--r--   0 user       (501) staff       (20)      197 2024-05-07 17:48:27.000000 docuscospacy-0.2.4/docuscospacy/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    26510 2024-05-07 18:07:19.000000 docuscospacy-0.2.4/docuscospacy/corpus_analysis.py
+-rw-r--r--   0 user       (501) staff       (20)    55200 2024-05-07 17:20:45.000000 docuscospacy-0.2.4/docuscospacy/corpus_utils.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-07 18:33:56.665393 docuscospacy-0.2.4/docuscospacy.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     4685 2024-05-07 18:33:56.000000 docuscospacy-0.2.4/docuscospacy.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      292 2024-05-07 18:33:56.000000 docuscospacy-0.2.4/docuscospacy.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-05-07 18:33:56.000000 docuscospacy-0.2.4/docuscospacy.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       86 2024-05-07 18:33:56.000000 docuscospacy-0.2.4/docuscospacy.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       13 2024-05-07 18:33:56.000000 docuscospacy-0.2.4/docuscospacy.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-05-07 18:33:56.666714 docuscospacy-0.2.4/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      961 2024-05-07 18:30:51.000000 docuscospacy-0.2.4/setup.py
```

### Comparing `docuscospacy-0.2.3/LICENSE` & `docuscospacy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docuscospacy-0.2.3/PKG-INFO` & `docuscospacy-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: docuscospacy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Support for spaCy models trained on DocuScope and the CLAWS7 tagset
 Home-page: https://github.com/browndw/docuscospacy
 Author: David Brown
 Author-email: dwb2@andrew.cmu.edu
 License: Apache License 2.0
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 |docuscope|
 
 docuscospacy: Support for spaCy models trained on DocuScope and the CLAWS7 tagset
 =================================================================================
@@ -94,8 +93,7 @@
 .. |rtd| image:: https://readthedocs.org/projects/docuscospacy/badge/?version=latest
     :target: https://docuscospacy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. |zenodo| image:: https://zenodo.org/badge/512227318.svg
     :target: https://zenodo.org/badge/latestdoi/512227318
     :alt: Citable Zenodo DOI
-
```

### Comparing `docuscospacy-0.2.3/README.rst` & `docuscospacy-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `docuscospacy-0.2.3/docuscospacy/corpus_analysis.py` & `docuscospacy-0.2.4/docuscospacy/corpus_analysis.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,67 @@
 """
 Functions for analyzing corpus data tagged with DocuScope and CLAWS7.
 .. codeauthor:: David Brown <dwb2d@andrew.cmu.edu>
 """
 
-from tmtoolkit.corpus import doc_tokens, kwic
-from tmtoolkit.tokenseq import pmi, pmi2, pmi3, index_windows_around_matches
 import numpy as np
 import pandas as pd
 import re
 from scipy.stats.distributions import chi2
+from tmtoolkit.corpus import doc_tokens
 from collections import Counter
 
-from .corpus_utils import _convert_totuple, _merge_tags, _merge_ds, _count_tags, _count_ds, _log_like, _log_ratio, _get_ngrams, _groupby_consecutive, _conlltags2tree, Tree
+from . corpus_utils import (
+	_convert_totuple, _merge_tags, _merge_ds, _count_tags, _count_ds, _log_like, _log_ratio, 
+	_PMI, _PMI2, _PMI3, _index_windows_around_matches, _tf_proportions, _tfidf, _get_ngrams, 
+	_groupby_consecutive, _conlltags2tree, Tree
+)
 
 def convert_corpus(tm_corpus):
     """
     A simple wrapper for coverting a tmtoolkit corpus in an nltk-like dictionary of tuples.
     
     :param tm_corpus: A tmtoolkit corpus
     :return: a dictionary of tuples
     """
     docs = doc_tokens(tm_corpus, with_attr=['token', 'whitespace', 'ent_iob', 'ent_type', 'tag'])
     tp = _convert_totuple(docs)
     d = {tm_corpus.doc_labels[i]: tp[i] for i in range(0,len(tp))}
     return(d)
  
+def normalize_dtm(dtm, scheme='prop'):
+    """
+    A function for converting a tags dtm to counts normalized by relative frequency or tf-idf
+    
+    :param dtm: A document-term-matrix with a doc_id column
+    :param scheme: One of 'prop' or 'tfidf' for normalizing counts
+    :return: a transformed dtm
+    """
+    dtm_norm = dtm.set_index('doc_id', inplace=False)
+    if scheme == 'prop':
+        dtm_norm = _tf_proportions(dtm_norm)
+    if scheme == 'tfidf':
+        dtm_norm = _tfidf(dtm_norm)
+    dtm_norm = dtm_norm.reset_index()
+    return(dtm_norm)
+
+def dtm_to_coo(dtm):
+    """
+    A function for converting a tags dtm to a COOrdinate format.
+    
+    :param dtm: A document-term-matrix with a doc_id column
+    :return: a COOrdinate format matrix, an index of document ids, and a list of variable names
+    """
+    docs = dtm['doc_id']
+    matrix_values = dtm.drop('doc_id', axis=1)
+    vocab = dtm.columns.values.tolist()[1:]
+    sparse_df = matrix_values.astype(pd.SparseDtype("float64", 0))
+    coo_sparse_matrix = sparse_df.sparse.to_coo()
+    return(coo_sparse_matrix, docs, vocab)
+
 def frequency_table(tok, n_tokens, count_by='pos'):
     """
     Generate a count of token frequencies.
     
     :param tok: A dictionary of tuples as generated by the convert_corpus function
     :param n_tokens: A count of total tokens against which to normalize
     :param count_by: One of 'pos' or 'ds' for aggregating tokens
@@ -111,72 +144,198 @@
         tag_counts.append(counts)
     df = pd.DataFrame.from_records(tag_counts)
     df = df.fillna(0)
     df = df.reindex(sorted(df.columns), axis=1)
     df.insert(0, 'doc_id', doc_id)
     return(df)
 
-def ngrams_table(tok, ng_span, n_tokens, count_by='pos'):
+def ngrams_by_token(tok, node_word: str, n_tokens, node_position=1, span=2, search_type='fixed', count_by='pos'):
     """
-    Generate a table of ngram frequencies.
+    Generate a table of ngram frequencies searching by token.
     
     :param tok: A dictionary of tuples as generated by the convert_corpus function
-    :param ng_span: An interger between 2 and 5 representing the size of the ngrams
+    :param node_word: A token to include in the n-grams
     :param n_tokens: A count of total tokens against which to normalize
+    :param node_position: The placement of the node word in the n-grams (1, for example, would be on the left)
+    :param span: An interger between 2 and 5 representing the size of the ngrams
+    :param search_type: One of 'fixed', 'starts_with', 'ends_with', or 'contains'
     :param count_by: One of 'pos' or 'ds' for aggregating tokens
     :return: a dataframe containing a token sequence the length of the span, a tag sequence the length of the span, absolute frequencies, normalized frequencies (per million tokens) and ranges
     """
-    tok = list(tok.values())
-    # set limit on the size of the ngrams
-    if ng_span < 2 or ng_span > 5:
+    if node_position > span:
+    	node_position = span
+    	print('Setting node position to right-most position in span.')
+    if span < 2 or span > 5:
         raise ValueError("Span must be < " + str(2) + " and > " + str(5))
+    if search_type not in ['fixed', 'starts_with', 'ends_with', 'contains']:
+    	raise ValueError('Search type must be on of fixed, starts_with, ends_with, or contains.')
+    span_l = node_position - 1
+    span_r = span - span_l
+    tok = list(tok.values())
     if count_by == 'pos':
-        mtp = _merge_tags(tok)
+        tc = _merge_tags(tok)
     if count_by == 'ds':
-        mtp = _merge_ds(tok)
-    ml = []
-    for i in range(0,len(mtp)):
-        ml.append(list('_tag_'.join(x) for x in mtp[i]))
-    tc = []
-    for i in range(0,len(ml)):
-        tc.append(list(_get_ngrams([x for x in ml[i]], n=ng_span)))
+        tc = _merge_ds(tok)
+    ngram_list = []
+    for i in range(0,len(tc)):
+        tp = tc[i]
+        tpf = [t[0] for t in tp]
+        # create a boolean vector for node word
+        if search_type == "fixed":
+            v = [t == node_word.lower() for t in tpf]
+        elif search_type == "starts_with":
+            v = [t.startswith(node_word.lower()) for t in tpf]
+        elif search_type == "ends_with":
+            v = [t.endswith(node_word.lower()) for t in tpf]
+        elif search_type == "contains":
+            v = [node_word.lower() in t.lower() for t in tpf]
+        if sum(v) > 0:
+            idx = list(_index_windows_around_matches(np.array(v), left=span_l, right=span_r, flatten=False))
+            start_idx = [min(x) for x in idx]
+            end_idx = [max(x) for x in idx]
+            in_span = []
+            for i in range(len(idx)):
+                span_tokens = [t for t in tp[start_idx[i]:end_idx[i]]]
+                in_span.append(span_tokens)
+                merged_tokens = []
+                for i in range(0,len(in_span)):
+                    if len(in_span[i]) == span:
+                        merged_tokens.append('_token_'.join(['_tag_'.join(x) for x in in_span[i]]))
+            ngram_list.append(merged_tokens)
+    # calculate ranges
     ngram_range = []
+    for i in range(0,len(ngram_list)):
+        ngram_range.append(list(set(ngram_list[i])))
+    ngram_range = [x for xs in ngram_range for x in xs]
+    ngram_range = Counter(ngram_range)
+    ngram_range = sorted(ngram_range.items(), key=lambda pair: pair[0], reverse=False)
+    # calculate counts
+    ngram_count = [x for xs in ngram_list for x in xs]
+    ngram_count = Counter(ngram_count)
+    ngram_count = sorted(ngram_count.items(), key=lambda pair: pair[0], reverse=False)
+    # build table
+    ngrams = [x[0] for x in ngram_count]
+    ngrams = [x.split('_token_') for x in ngrams]
+    ngrams = [sum([x[i].split('_tag_') for i in range(span)], []) for x in ngrams]
+    order = list(range(0, span*2, 2)) + list(range(1, span*2 + 1, 2))
+    for l in reversed(range(len(ngrams))):
+        ngrams[l] = [ngrams[l][j] for j in order]
+    ngrams = np.array(ngrams)
+    ngram_freq = np.array([x[1] for x in ngram_count])
+    ngram_prop = np.array(ngram_freq)/n_tokens*1000000
+    ngram_range = np.array([x[1] for x in ngram_range])/len(tok)*100
+    counts = list(zip(ngrams.tolist(), ngram_freq.tolist(), ngram_prop.tolist(), ngram_range.tolist()))
+    ngram_counts = list()
+    for x in counts:
+        tt = tuple()
+        for y in x:
+            if not type(y) == list:
+                tt += (y,)
+            else:
+                tt += (*y,)
+        ngram_counts.append(tt)
+    df = pd.DataFrame(ngram_counts, columns=['Token' + str(i) for i in range (1, span+1)] + ['Tag' + str(i) for i in range (1, span+1)] + ['AF', 'RF', 'Range'])
+    df.sort_values(by=['AF', 'Token1'], ascending=[False, True], inplace=True)
+    df.reset_index(drop=True, inplace=True)
+    if df.empty:
+    	print('Your n-gram search did not return any results.')
+    else:
+    	return(df)
+
+def ngrams_by_tag(tok, tag: str, n_tokens, tag_position = 1, span = 2, search_type='fixed', count_by='pos'):
+    """
+    Generate a table of ngram frequencies searching by tag.
+    
+    :param tok: A dictionary of tuples as generated by the convert_corpus function
+    :param tag: A tag to include in the n-grams
+    :param n_tokens: A count of total tokens against which to normalize
+    :param tag_position: The placement of tag in the n-grams (1, for example, would be on the left)
+    :param span: An interger between 2 and 5 representing the size of the ngrams
+    :param search_type: One of 'fixed', 'starts_with', 'ends_with', or 'contains'
+    :param count_by: One of 'pos' or 'ds' for aggregating tokens
+    :return: a dataframe containing a token sequence the length of the span, a tag sequence the length of the span, absolute frequencies, normalized frequencies (per million tokens) and ranges
+    """
+    if tag_position > span:
+    	tag_position = span
+    	print('Setting node position to right-most position in span.')
+    if span < 2 or span > 5:
+        raise ValueError("Span must be < " + str(2) + " and > " + str(5))
+    span_l = tag_position - 1
+    span_r = span - span_l
+    tok = list(tok.values())
+    if count_by == 'pos':
+        tc = _merge_tags(tok)
+    if count_by == 'ds':
+        tc = _merge_ds(tok)
+    ngram_list = []
     for i in range(0,len(tc)):
-        ngram_range.append(list(set(tc[i])))
+        tp = tc[i]
+        tpf = [t[1] for t in tp]
+        # create a boolean vector for tag
+        # create a boolean vector for node word
+        if search_type == "fixed":
+            v = [t.lower() == tag.lower() for t in tpf]
+        elif search_type == "starts_with":
+            v = [t.lower().startswith(tag.lower()) for t in tpf]
+        elif search_type == "ends_with":
+            v = [t.lower().endswith(tag.lower()) for t in tpf]
+        elif search_type == "contains":
+            v = [tag.lower() in t.lower() for t in tpf]
+        if sum(v) > 0:
+            idx = list(_index_windows_around_matches(np.array(v), left=span_l, right=span_r, flatten=False))
+            start_idx = [min(x) for x in idx]
+            end_idx = [max(x) for x in idx]
+            in_span = []
+            for i in range(len(idx)):
+                span_tokens = [t for t in tp[start_idx[i]:end_idx[i]]]
+                in_span.append(span_tokens)
+                merged_tokens = []
+                for i in range(0,len(in_span)):
+                    if len(in_span[i]) == span:
+                        merged_tokens.append('_token_'.join(['_tag_'.join(x) for x in in_span[i]]))
+            ngram_list.append(merged_tokens)
+    # calculate ranges
+    ngram_range = []
+    for i in range(0,len(ngram_list)):
+        ngram_range.append(list(set(ngram_list[i])))
     ngram_range = [x for xs in ngram_range for x in xs]
     ngram_range = Counter(ngram_range)
     ngram_range = sorted(ngram_range.items(), key=lambda pair: pair[0], reverse=False)
-    ngram_list = [x for xs in tc for x in xs]
-    ngram_list = Counter(ngram_list)
-    ngram_list = sorted(ngram_list.items(), key=lambda pair: pair[0], reverse=False)
-    ngrams = [x[0] for x in ngram_list]
-    ngrams = [sum([x[i].split('_tag_') for i in range(ng_span)], []) for x in ngrams]
-    order = list(range(0, ng_span*2, 2)) + list(range(1, ng_span*2 + 1, 2))
+    # calculate counts
+    ngram_count = [x for xs in ngram_list for x in xs]
+    ngram_count = Counter(ngram_count)
+    ngram_count = sorted(ngram_count.items(), key=lambda pair: pair[0], reverse=False)
+    # build table
+    ngrams = [x[0] for x in ngram_count]
+    ngrams = [x.split('_token_') for x in ngrams]
+    ngrams = [sum([x[i].split('_tag_') for i in range(span)], []) for x in ngrams]
+    order = list(range(0, span*2, 2)) + list(range(1, span*2 + 1, 2))
     for l in reversed(range(len(ngrams))):
         ngrams[l] = [ngrams[l][j] for j in order]
     ngrams = np.array(ngrams)
-    ngram_freq = np.array([x[1] for x in ngram_list])
-    # total_ngrams = sum(ngram_freq)
-    # Note: using non_punct for normalization
+    ngram_freq = np.array([x[1] for x in ngram_count])
     ngram_prop = np.array(ngram_freq)/n_tokens*1000000
     ngram_range = np.array([x[1] for x in ngram_range])/len(tok)*100
     counts = list(zip(ngrams.tolist(), ngram_freq.tolist(), ngram_prop.tolist(), ngram_range.tolist()))
     ngram_counts = list()
     for x in counts:
         tt = tuple()
         for y in x:
             if not type(y) == list:
                 tt += (y,)
             else:
                 tt += (*y,)
         ngram_counts.append(tt)
-    ngram_counts = pd.DataFrame(ngram_counts, columns=['Token' + str(i) for i in range (1, ng_span+1)] + ['Tag' + str(i) for i in range (1, ng_span+1)] + ['AF', 'RF', 'Range'])
-    ngram_counts.sort_values(by=['AF', 'Token1'], ascending=[False, True], inplace=True)
-    ngram_counts.reset_index(drop=True, inplace=True)
-    return(ngram_counts)
+    df = pd.DataFrame(ngram_counts, columns=['Token' + str(i) for i in range (1, span+1)] + ['Tag' + str(i) for i in range (1, span+1)] + ['AF', 'RF', 'Range'])
+    df.sort_values(by=['AF', 'Token1'], ascending=[False, True], inplace=True)
+    df.reset_index(drop=True, inplace=True)
+    if df.empty:
+    	print('Your n-gram search did not return any results.')
+    else:
+    	return(df)
 
 def coll_table(tok, node_word, l_span=4, r_span=4, statistic='pmi', count_by='pos', node_tag=None, tag_ignore=False):
     """
     Generate a table of collocations by association measure.
     
     :param tok: A dictionary of tuples as generated by the convert_corpus function
     :param node_word: The token around with collocations are measured
@@ -208,15 +367,15 @@
         # create a boolean vector for node word
         if node_tag is None:
             v = [t[0] == node_word for t in tpf]
         else:
             v = [t[0] == node_word and t[1].startswith(node_tag) for t in tpf]
         if sum(v) > 0:
             # get indices within window around the node
-            idx = list(index_windows_around_matches(np.array(v), left=l_span, right=r_span, flatten=False))
+            idx = list(_index_windows_around_matches(np.array(v), left=l_span, right=r_span, flatten=False))
             node_idx = [i for i, x in enumerate(v) if x == True]
             # remove node word from collocates
             coll_idx = [np.setdiff1d(idx[i], node_idx[i]) for i in range(len(idx))]
             coll_idx = [x for xs in coll_idx for x in xs]
             coll = [tpf[i] for i in coll_idx]
         else:
             coll = []
@@ -242,73 +401,98 @@
     else:
         node_freq = sum(df_total[(df_total['Token'] == node_word) & (df_total['Tag'].str.startswith(node_tag, na=False))]['Freq Total'])
     if bool(tag_ignore) == True:
         df = pd.merge(df_span, df_total, how='inner', on=['Token'])
     else:
         df = pd.merge(df_span, df_total, how='inner', on=['Token', 'Tag'])
     if statistic=='pmi':
-        df['MI'] = pmi(node_freq, df['Freq Total'], df['Freq Span'], sum(df_total['Freq Total']), normalize=False)
+        df['MI'] = _PMI(node_freq, df['Freq Total'], df['Freq Span'], sum(df_total['Freq Total']), normalize=False)
     if statistic=='npmi':
-        df['MI'] = pmi(node_freq, df['Freq Total'], df['Freq Span'], sum(df_total['Freq Total']), normalize=True)
+        df['MI'] = _PMI(node_freq, df['Freq Total'], df['Freq Span'], sum(df_total['Freq Total']), normalize=True)
     if statistic=='pmi2':
-        df['MI'] = pmi2(node_freq, df['Freq Total'], df['Freq Span'], sum(df_total['Freq Total']))
+        df['MI'] = _PMI2(node_freq, df['Freq Total'], df['Freq Span'], sum(df_total['Freq Total']))
     if statistic=='pmi3':
-        df['MI'] = pmi3(node_freq, df['Freq Total'], df['Freq Span'], sum(df_total['Freq Total']))
+        df['MI'] = _PMI3(node_freq, df['Freq Total'], df['Freq Span'], sum(df_total['Freq Total']))
     df.sort_values(by=['MI', 'Token'], ascending=[False, True], inplace=True)
     df.reset_index(drop=True, inplace=True)
     return(df)
 
-def kwic_center_node(tm_corpus, node_word,  ignore_case=True, glob=False):
+def kwic_center_node(tok, node_word, ignore_case=True, search_type='fixed'):
     """
     Generate a KWIC table with the node word in the center column.
     
-    :param tm_corpus: A tmtoolkit corpus
+    :param tok: A dictionary of tuples as generated by the convert_corpus function
     :param node_word: The token of interest
-    :param ignore_case: If set to False, search will be case sensitive
-    :param glob: If set to True, glob-style searching is enabled
+    :param search_type: One of 'fixed', 'starts_with', 'ends_with', or 'contains'
     :return: a dataframe with the node word in a center column and context columns on either side.
     """
-    if bool(glob)==False:
-        kl = kwic(tm_corpus, node_word, context_size=10, ignore_case=ignore_case, highlight_keyword="##")
+    kwic = []
+    for i in range(0,len(tok)):
+        tpf = list(tok.values())[i]
+        doc_id = list(tok.keys())[i]
+        # create a boolean vector for node word
+        if bool(ignore_case) == True and search_type == "fixed":
+            v = [t[0].strip().lower() == node_word.lower() for t in tpf]
+        elif bool(ignore_case) == False and search_type == "fixed":
+            v = [t[0].strip() == node_word for t in tpf]
+        elif bool(ignore_case) == True and search_type == "starts_with":
+            v = [t[0].strip().lower().startswith(node_word.lower()) for t in tpf]
+        elif bool(ignore_case) == False and search_type == "starts_with":
+            v = [t[0].strip().startswith(node_word) for t in tpf]
+        elif bool(ignore_case) == True and search_type == "ends_with":
+            v = [t[0].strip().lower().endswith(node_word.lower()) for t in tpf]
+        elif bool(ignore_case) == False and search_type == "ends_with":
+            v = [t[0].strip().endswith(node_word) for t in tpf]
+        elif bool(ignore_case) == True and search_type == "contains":
+            v = [node_word.lower() in t[0].strip().lower() for t in tpf]
+        elif bool(ignore_case) == False and search_type == "contains":
+            v = [node_word in t[0].strip() for t in tpf]
+
+        if sum(v) > 0:
+            # get indices within window around the node
+            idx = list(_index_windows_around_matches(np.array(v), left=7, right=7, flatten=False))
+            node_idx = [i for i, x in enumerate(v) if x == True]
+            start_idx = [min(x) for x in idx]
+            end_idx = [max(x) for x in idx]
+            in_span = []
+            for i in range(len(node_idx)):
+                pre_node = "".join([t[0] for t in tpf[start_idx[i]:node_idx[i]]]).strip()
+                post_node = "".join([t[0] for t in tpf[node_idx[i]+1:end_idx[i]]]).strip()
+                node = tpf[node_idx[i]][0]
+                in_span.append((doc_id, pre_node, node, post_node))
+            kwic.append(in_span)
+    kwic = [x for xs in kwic for x in xs]
+    if len(kwic) > 0:
+        df = pd.DataFrame(kwic)
+        df.columns =['Doc ID', 'Pre-Node', 'Node', 'Post-Node']
     else:
-        kl = kwic(tm_corpus, node_word, context_size=10, ignore_case=ignore_case, match_type='glob', highlight_keyword="##")
-    keys = [k for k in kl.keys() for v in kl[k]]
-    token_list = [v for k in kl.keys() for v in kl[k]]
-    node_idx = [i for x in range(len(token_list)) for i in range(len(token_list[x])) if token_list[x][i].startswith('##') and token_list[x][i].endswith('##') and len(token_list[x][i]) > 2]
-    pre_node = [' '.join(token_list[i][:node_idx[i]]) for i in range(len(token_list))]
-    # set a span after which characters are trimmed for display
-    pre_node = [('..' + l[len(l)-75:]) if len(l) > 75 else l for l in pre_node]
-    node = [token_list[i][node_idx[i]].replace('##', '') for i in range(len(token_list))]
-    post_node = [' '.join(token_list[i][node_idx[i] + 1:]) for i in range(len(token_list))]
-    # apply same trim span
-    post_node = [(l[:75] + '..') if len(l) > 75 else l for l in post_node]
-    df = pd.DataFrame.from_dict({'Doc': keys, 'Pre-Node': pre_node, 'Node': node, 'Post-Node': post_node})
+        df = ''
+        print('Your KWIC search did not return any results.')
     return(df)
 
-
 def keyness_table(target_counts, ref_counts, correct=False, tags_only=False):
     """
     Generate a keyness table comparing token frequencies from a taget and a reference corpus
     
     :param target_counts: A frequency table from a target corpus
     :param ref_counts: A frequency table from a reference corpus
     :param correct: If True, apply the Yates correction to the log-likelihood calculation
     :param tags_only: If True, it is assumed the frequency tables are of the type produce by the tags_table function
     :return: a dataframe of absolute frequencies, normalized frequencies (per million tokens) and ranges for both corpora, as well as keyness values as calculated by log-likelihood and effect size as calculated by Log Ratio.
     """
     total_target = target_counts['AF'].sum()
     total_reference = ref_counts['AF'].sum()
     if bool(tags_only) == True:
-        df_1 = target_counts.set_axis(['Tag','AF', 'RF', 'Range'], axis=1, inplace=False)
+        df_1 = target_counts.set_axis(['Tag','AF', 'RF', 'Range'], axis=1)
     else:
-        df_1 = target_counts.set_axis(['Token', 'Tag','AF', 'RF', 'Range'], axis=1, inplace=False)
+        df_1 = target_counts.set_axis(['Token', 'Tag','AF', 'RF', 'Range'], axis=1)
     if bool(tags_only) == True:
-        df_2 = ref_counts.set_axis(['Tag', 'AF Ref', 'RF Ref', 'Range Ref'], axis=1, inplace=False)
+        df_2 = ref_counts.set_axis(['Tag', 'AF Ref', 'RF Ref', 'Range Ref'], axis=1)
     else:
-        df_2 = ref_counts.set_axis(['Token', 'Tag', 'AF Ref', 'RF Ref', 'Range Ref'], axis=1, inplace=False)
+        df_2 = ref_counts.set_axis(['Token', 'Tag', 'AF Ref', 'RF Ref', 'Range Ref'], axis=1)
     if bool(tags_only) == True:
         df = pd.merge(df_1, df_2, how='outer', on=['Tag'])
     else:
         df = pd.merge(df_1, df_2, how='outer', on=['Token', 'Tag'])
     df.fillna(0, inplace=True)
     if bool(correct) == True:
         df['LL'] = np.vectorize(_log_like)(df['AF'], df['AF Ref'], total_target, total_reference, correct=True)
```

### Comparing `docuscospacy-0.2.3/docuscospacy/corpus_utils.py` & `docuscospacy-0.2.4/docuscospacy/corpus_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 
 .. codeauthor:: David Brown <dwb2@andrew.cmu.edu>
 """
 
 import string
 import re
 import numpy as np
+from functools import partial
 from itertools import groupby, islice
 from collections import Counter
 from operator import itemgetter
+from typing import Union, List, Callable, Optional
 
 def _convert_totuple(tok):
     """
     Convert a tmtoolkit tokens object to a tuple of the nltk-type: [(token), (tag), (iob-ent)].
     
     :param tok: a tmtoolkit tokens object
     """
@@ -43,14 +45,75 @@
     
     :param lst: a list
     """
     for _, g in groupby(enumerate(lst), lambda x: x[0] - x[1]):
         yield list(map(itemgetter(1), g))
 
 
+# https://github.com/WZBSocialScienceCenter/tmtoolkit/blob/master/tmtoolkit/tokenseq.py
+def _index_windows_around_matches(matches: np.ndarray, left: int, right: int,
+                                 flatten: bool = False, remove_overlaps: bool = True) \
+        -> Union[List[List[int]], np.ndarray]:
+    """
+    Take a boolean 1D array `matches` of length N and generate an array of indices, where each occurrence of a True
+    value in the boolean vector at index i generates a sequence of the form:
+
+    .. code-block:: text
+
+        [i-left, i-left+1, ..., i, ..., i+right-1, i+right, i+right+1]
+
+    If `flatten` is True, then a flattened NumPy 1D array is returned. Otherwise, a list of NumPy arrays is returned,
+    where each array contains the window indices.
+
+    `remove_overlaps` is only applied when `flatten` is True.
+
+    Example with ``left=1 and right=1, flatten=False``:
+
+    .. code-block:: text
+
+        input:
+        #   0      1      2      3     4      5      6      7     8
+        [True, True, False, False, True, False, False, False, True]
+        output (matches *highlighted*):
+        [[0, *1*], [0, *1*, 2], [3, *4*, 5], [7, *8*]]
+
+    Example with ``left=1 and right=1, flatten=True, remove_overlaps=True``:
+
+    .. code-block:: text
+
+        input:
+        #   0      1      2      3     4      5      6      7     8
+        [True, True, False, False, True, False, False, False, True]
+        output (matches *highlighted*, other values belong to the respective "windows"):
+        [*0*, *1*, 2, 3, *4*, 5, 7, *8*]
+    """
+    if not isinstance(matches, np.ndarray) or matches.dtype != bool:
+        raise ValueError('`matches` must be a boolean NumPy array')
+    if not isinstance(left, int) or left < 0:
+        raise ValueError('`left` must be an integer >= 0')
+    if not isinstance(right, int) or right < 0:
+        raise ValueError('`right` must be an integer >= 0')
+
+    ind = np.where(matches)[0]
+    nested_ind = list(map(lambda x: np.arange(x - left, x + right + 1), ind))
+
+    if flatten:
+        if not nested_ind:
+            return np.array([], dtype=int)
+
+        window_ind = np.concatenate(nested_ind)
+        window_ind = window_ind[(window_ind >= 0) & (window_ind < len(matches))]
+
+        if remove_overlaps:
+            return np.sort(np.unique(window_ind))
+        else:
+            return window_ind
+    else:
+        return [w[(w >= 0) & (w < len(matches))] for w in nested_ind]
+
 def _merge_tags(tok):
     """
     Merge part-of-speech tag sequences into a single token like 'for example' or 'in spite of'.
     
     :param tok: a tokens tuple object
     """
     tok = [[(word.lower(), tag, ds) for word, tag, ds in element] for element in tok]
@@ -231,14 +294,196 @@
     """
     percent_a = 0.5 / total_target if n_target == 0 else n_target/total_target
     percent_b = 0.5 / total_reference if n_reference == 0 else n_reference/total_reference
     ratio = np.log2(percent_a / percent_b)
     return(ratio)
 
 
+# https://github.com/WZBSocialScienceCenter/tmtoolkit/blob/master/tmtoolkit/tokenseq.py
+def _PMI(x: np.ndarray, y: np.ndarray, xy: np.ndarray, n_total: Optional[int] = None, logfn: Callable = np.log2,
+        k: int = 1, normalize: bool = False) -> np.ndarray:
+    """
+    Calculate pointwise mutual information measure (PMI) either from probabilities p(x), p(y), p(x, y) given as `x`,
+    `y`, `xy`, or from total counts `x`, `y`, `xy` and additionally `n_total`. Setting `k` > 1 gives PMI^k variants.
+    Setting `normalized` to True gives normalized PMI (NPMI) as in [Bouma2009]_. See [RoleNadif2011]_ for a comparison
+    of PMI variants.
+
+    Probabilities should be such that ``p(x, y) <= min(p(x), p(y))``.
+
+    :param x: probabilities p(x) or count of occurrence of x (interpreted as count if `n_total` is given)
+    :param y: probabilities p(y) or count of occurrence of y (interpreted as count if `n_total` is given)
+    :param xy: probabilities p(x, y) or count of occurrence of x *and* y (interpreted as count if `n_total` is given)
+    :param n_total: if given, `x`, `y` and `xy` are interpreted as counts with `n_total` as size of the sample space
+    :param logfn: logarithm function to use (default: ``np.log`` – natural logarithm)
+    :param k: if `k` > 1, calculate PMI^k variant
+    :param normalize: if True, normalize to range [-1, 1]; gives NPMI measure
+    :return: array with same length as inputs containing (N)PMI measures for each input probability
+    """
+    if not isinstance(k, int) or k < 1:
+        raise ValueError('`k` must be a strictly positive integer')
+
+    if k > 1 and normalize:
+        raise ValueError('normalization is only implemented for standard PMI with `k=1`')
+
+    if n_total is not None:
+        if n_total < 1:
+            raise ValueError('`n_total` must be strictly positive')
+        x = x/n_total
+        y = y/n_total
+        xy = xy/n_total
+
+    pmi_val = logfn(xy) - logfn(x * y)
+
+    if k > 1:
+        return pmi_val - (1-k) * logfn(xy)
+    else:
+        if normalize:
+            return pmi_val / -logfn(xy)
+        else:
+            return pmi_val
+
+_NPMI = partial(_PMI, k=1, normalize=True)
+_PMI2 = partial(_PMI, k=2, normalize=False)
+_PMI3 = partial(_PMI, k=3, normalize=False)
+
+# https://github.com/WZBSocialScienceCenter/tmtoolkit/blob/master/tmtoolkit/bow/bow_stats.py
+def _doc_frequencies(dtm, min_val=1, proportions=0):
+    """
+    For each term in the vocab of `dtm` (i.e. its columns), return how often it occurs at least `min_val` times per
+    document.
+
+    :param dtm: (sparse) document-term-matrix of size NxM (N docs, M is vocab size) with raw term counts.
+    :param min_val: threshold for counting occurrences
+    :param proportions: one of :attr:`~tmtoolkit.types.Proportion`: ``NO (0)`` – return counts; ``YES (1)`` – return
+                        proportions; ``LOG (2)`` – return log of proportions
+    :return: NumPy array of size M (vocab size) indicating how often each term occurs at least `min_val` times.
+    """
+    if dtm.ndim != 2:
+        raise ValueError('`dtm` must be a 2D array/matrix')
+
+    doc_freq = np.sum(dtm >= min_val, axis=0)
+
+    if doc_freq.ndim != 1:
+        doc_freq = doc_freq.A.flatten()
+
+    if proportions == 1:
+        return doc_freq / dtm.shape[0]
+    elif proportions == 2:
+        return np.log(doc_freq) - np.log(dtm.shape[0])
+    else:
+        return doc_freq
+
+def _doc_lengths(dtm):
+    """
+    Return the length, i.e. number of terms for each document in document-term-matrix `dtm`.
+    This corresponds to the row-wise sums in `dtm`.
+
+    :param dtm: (sparse) document-term-matrix of size NxM (N docs, M is vocab size) with raw terms counts
+    :return: NumPy array of size N (number of docs) with integers indicating the number of terms per document
+    """
+    if dtm.ndim != 2:
+        raise ValueError('`dtm` must be a 2D array/matrix')
+
+    res = np.sum(dtm, axis=1)
+    if res.ndim != 1:
+        return res.A.flatten()
+    else:
+        return res
+
+def _tf_proportions(dtm, norm=False, scale=False):
+    """
+    Transform raw count document-term-matrix `dtm` to term frequency matrix with proportions, i.e. term counts
+    normalized by document length.
+
+    Note that this may introduce NaN values due to division by zero when a document is of length 0.
+
+    :param dtm: (sparse) document-term-matrix of size NxM (N docs, M is vocab size) with raw term counts
+    :return: (sparse) term frequency matrix of size NxM with proportions, i.e. term counts normalized by document length
+    """
+
+    norm_factor = 1 / np.array(_doc_lengths(dtm))[:, None]   # shape: Nx1
+
+    res = dtm * norm_factor
+    
+    if norm == True:
+        res *=100
+    else:
+        res
+    if scale == True:
+        scaled_res = res.select_dtypes(include='number').apply(scipy.stats.zscore)
+        res = pd.DataFrame(scaled_res, index=res.index, columns=res.columns)
+    else:
+        res
+    if isinstance(res, np.matrix):
+        return res.A
+    else:
+        return res
+
+def _idf(dtm, smooth_log=1, smooth_df=1):
+    """
+    Calculate inverse document frequency (idf) vector from raw count document-term-matrix `dtm` with formula
+    ``log(smooth_log + N / (smooth_df + df))``, where ``N`` is the number of documents, ``df`` is the document frequency
+    (see function :func:`~tmtoolkit.bow.bow_stats.doc_frequencies`), `smooth_log` and `smooth_df` are smoothing
+    constants. With default arguments, the formula is thus ``log(1 + N/(1+df))``.
+
+    Note that this may introduce NaN values due to division by zero when a document is of length 0.
+
+    :param dtm: (sparse) document-term-matrix of size NxM (N docs, M is vocab size) with raw term counts.
+    :param smooth_log: smoothing constant inside log()
+    :param smooth_df: smoothing constant to add to document frequency
+    :return: NumPy array of size M (vocab size) with inverse document frequency for each term in the vocab
+    """
+    if dtm.ndim != 2 or 0 in dtm.shape:
+        raise ValueError('`dtm` must be a non-empty 2D array/matrix')
+
+    n_docs = dtm.shape[0]
+    df = _doc_frequencies(dtm)
+
+    if smooth_log == smooth_df == 1:      # log1p is faster than the equivalent log(1 + x)
+        # log(1 + N/(1+df)) = log((1+df+N)/(1+df)) = log(1+df+N) - log(1+df) = log1p(df+N) - log1p(df)
+        return np.log1p(df + n_docs) - np.log1p(df)
+    else:
+        # with s = smooth_log and t = smooth_df
+        # log(s + N/(t+df)) = log((s(t+df)+N)/(t+df)) = log(s(t+df)+N) - log(t+df)
+        return np.log(smooth_log * (smooth_df + df) + n_docs) - np.log(smooth_df + df)
+
+
+def _tfidf(dtm, tf_func=_tf_proportions, idf_func=_idf, **kwargs):
+    """
+    Calculate tfidf (term frequency inverse document frequency) matrix from raw count document-term-matrix `dtm` with
+    matrix multiplication ``tf * diag(idf)``, where `tf` is the term frequency matrix ``tf_func(dtm)`` and ``idf`` is
+    the document frequency vector ``idf_func(dtm)``.
+
+    :param dtm: (sparse) document-term-matrix of size NxM (N docs, M is vocab size) with raw term counts
+    :param tf_func: function to calculate term-frequency matrix; see ``tf_*`` functions in this module
+    :param idf_func: function to calculate inverse document frequency vector; see ``tf_*`` functions in this module
+    :param kwargs: additional parameters passed to `tf_func` or `idf_func` like `K` or `smooth` (depending on which
+                   parameters these functions except)
+    :return: (sparse) tfidf matrix of size NxM
+    """
+    if dtm.ndim != 2 or 0 in dtm.shape:
+        raise ValueError('`dtm` must be a non-empty 2D array/matrix')
+
+    if idf_func is _idf:
+        idf_opts = {}
+        if 'smooth_log' in kwargs:
+            idf_opts['smooth_log'] = kwargs.pop('smooth_log')
+        if 'smooth_df' in kwargs:
+            idf_opts['smooth_df'] = kwargs.pop('smooth_df')
+
+        idf_vec = idf_func(dtm, **idf_opts)
+    elif idf_func is idf_probabilistic and 'smooth' in kwargs:
+        idf_vec = idf_func(dtm, smooth=kwargs.pop('smooth'))
+    else:
+        idf_vec = idf_func(dtm)
+
+    tf_mat = tf_func(dtm, **kwargs)
+
+    return tf_mat * idf_vec
+
 def _conlltags2tree(
     sentence, chunk_types=("NP", "PP", "VP"), root_label="S", strict=False
 ):
     """
     Convert the CoNLL IOB format to a tree.
     """
     tree = Tree(root_label, [])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `docuscospacy-0.2.3/docuscospacy.egg-info/PKG-INFO` & `docuscospacy-0.2.4/docuscospacy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: docuscospacy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Support for spaCy models trained on DocuScope and the CLAWS7 tagset
 Home-page: https://github.com/browndw/docuscospacy
 Author: David Brown
 Author-email: dwb2@andrew.cmu.edu
 License: Apache License 2.0
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 |docuscope|
 
 docuscospacy: Support for spaCy models trained on DocuScope and the CLAWS7 tagset
 =================================================================================
@@ -94,8 +93,7 @@
 .. |rtd| image:: https://readthedocs.org/projects/docuscospacy/badge/?version=latest
     :target: https://docuscospacy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 .. |zenodo| image:: https://zenodo.org/badge/512227318.svg
     :target: https://zenodo.org/badge/latestdoi/512227318
     :alt: Citable Zenodo DOI
-
```

### Comparing `docuscospacy-0.2.3/setup.py` & `docuscospacy-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.2.3'
+VERSION = '0.2.4'
 PACKAGE_NAME = 'docuscospacy'
 AUTHOR = 'David Brown'
 AUTHOR_EMAIL = 'dwb2@andrew.cmu.edu'
 URL = 'https://github.com/browndw/docuscospacy'
 
 LICENSE = 'Apache License 2.0'
 DESCRIPTION = 'Support for spaCy models trained on DocuScope and the CLAWS7 tagset'
```

