# Comparing `tmp/probabilistic_word_embeddings-1.2.0.tar.gz` & `tmp/probabilistic_word_embeddings-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probabilistic_word_embeddings-1.2.0.tar", max compression
+gzip compressed data, was "probabilistic_word_embeddings-1.2.1.tar", max compression
```

## Comparing `probabilistic_word_embeddings-1.2.0.tar` & `probabilistic_word_embeddings-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     3406 2023-01-18 15:20:33.692173 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/__init__.py
--rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/Card-660.tsv
--rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MC-30.tsv
--rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
--rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
--rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
--rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/RG-65.tsv
--rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
--rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv
--rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
--rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
--rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
--rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
--rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/YP-130.tsv
--rw-r--r--   0        0        0     7424 2023-04-25 13:31:30.609859 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/embeddings.py
--rw-r--r--   0        0        0     9733 2023-04-25 14:14:16.286882 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/estimation.py
--rwxr-xr-x   0        0        0     9826 2023-04-25 13:31:30.614433 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/evaluation.py
--rw-r--r--   0        0        0     3551 2023-04-25 13:31:30.615164 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/models.py
--rw-r--r--   0        0        0     4915 2023-04-25 13:31:30.615879 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/preprocessing.py
--rw-r--r--   0        0        0     3492 2023-04-25 13:31:30.616555 probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/utils.py
--rw-r--r--   0        0        0      473 2023-04-25 14:20:07.081905 probabilistic_word_embeddings-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.2.0/setup.py
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3406 2023-01-18 15:20:33.692173 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/__init__.py
+-rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/Card-660.tsv
+-rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/MC-30.tsv
+-rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
+-rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
+-rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
+-rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/RG-65.tsv
+-rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
+-rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/SimLex999.tsv
+-rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
+-rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
+-rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
+-rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
+-rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/YP-130.tsv
+-rw-r--r--   0        0        0     7424 2023-04-25 13:31:30.609859 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/embeddings.py
+-rw-r--r--   0        0        0     9750 2023-04-26 08:35:50.582614 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/estimation.py
+-rwxr-xr-x   0        0        0     9851 2023-04-27 11:29:34.593807 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/evaluation.py
+-rw-r--r--   0        0        0     3551 2023-04-25 13:31:30.615164 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/models.py
+-rw-r--r--   0        0        0     5471 2023-04-25 14:40:29.826311 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/preprocessing.py
+-rw-r--r--   0        0        0     3492 2023-04-25 13:31:30.616555 probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/utils.py
+-rw-r--r--   0        0        0      473 2023-04-27 11:28:15.515594 probabilistic_word_embeddings-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.2.1/setup.py
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.2.1/PKG-INFO
```

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/__init__.py` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/Card-660.tsv` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/Card-660.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MC-30.tsv` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/MC-30.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MTurk-287.tsv` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/MTurk-287.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/MTurk-771.tsv` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/MTurk-771.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/RG-65.tsv` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/RG-65.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/SimLex999.tsv` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/SimLex999.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/data/eval/YP-130.tsv` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/data/eval/YP-130.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/embeddings.py` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/embeddings.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/estimation.py` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/estimation.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
             i,j,x  = generate_batch(data, model=model, ws=ws, ns=ns, batch_size=batch_size, start_ix=start_ix)
 
             with tf.GradientTape() as tape:
                 if model == "cbow":
                     log_prob = tf.reduce_sum(cbow_likelihood(e, i, j, x=x)) + e.log_prob(batch_size, N)
                 elif model == "sgns":
                     log_prob = tf.reduce_sum(sgns_likelihood(e, i, j, x=x)) + e.log_prob(batch_size, N)
-                epoch_logprobs.append(log_prob)
+                epoch_logprobs.append(log_prob * N / batch_size)
                 d_l_d_theta = -tape.gradient(log_prob, embedding.theta) * N / batch_size
             
             d_l_d_q_mean = d_l_d_theta
             d_l_q_std_log = tf.multiply(tf.multiply(d_l_d_theta, epsilon), tf.math.exp(q_std_log))
 
             # Add the entropy term
             d_l_q_std_log = d_l_q_std_log - tf.ones(d_l_q_std_log.shape, dtype=tf.float64)
```

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/evaluation.py` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,40 +118,40 @@
         corr, p_value = rank_correlation(merged_df["similarity_x"], merged_df["similarity_y"])
 
         rows.append([dataset, corr, len(merged_df), p_value])
         #print(f"Rank Correlation {corr}")
 
     return pd.DataFrame(rows, columns=["Dataset", "Rank Correlation", "No. of Observations", "p-value"])
 
-def nearest_neighbors(embedding, words, K=25):
+def nearest_neighbors(embedding, words, K=25, epsilon=0.00001):
     """
     Evaluate embedding performance on word analogy tasks.
     
     Args:
         embedding: embedding as pwe.embeddings.Embedding
         dataset (pd.DataFrame): Dataframe where each row has four words, word1 - word2 + word3 ≈ word4
     """
     e = copy.deepcopy(embedding)
     words = [wd for wd in words if wd in embedding]
     r = len(words)
     X = embedding[words]
 
     inv_vocab = {v: k for k, v in e.vocabulary.items()}
     eliminate = list(range(len(inv_vocab)))
-    eliminate = [0.0 if ("_c" in inv_vocab[i] or inv_vocab[i] in words) else 1.0 for i in eliminate]
+    eliminate = [-100.0 if ("_c" in inv_vocab[i] or inv_vocab[i] in words) else 0.0 - epsilon for i in eliminate]
     eliminate = tf.transpose(tf.constant([eliminate], dtype=tf.float64))
 
     X, _ = tf.linalg.normalize(X, axis=1)
 
     theta, _ = tf.linalg.normalize(e.theta, axis=1)
     e.theta.assign(theta)
 
     Ex = tf.linalg.tensordot(e.theta, X, axes=[1,1])
     tiled_eliminate = tf.tile(eliminate, [1,r])
-    Ex = tf.multiply(Ex, tiled_eliminate)
+    Ex = tf.add(Ex, tiled_eliminate)
 
     rows = []
 
     for i in range(r):
         y_hat = Ex[:,i]
         _, tops = tf.math.top_k(y_hat, k=K)
         topwords = [inv_vocab[int(i)] for i in tops]
```

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/models.py` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/models.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/preprocessing.py` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,48 +72,56 @@
             kepts = rands > probs
             indices = tf.where(kepts)
             newdata = tf.gather_nd(chunk, indices)
             l = l + [wd.decode("utf-8") for wd in newdata.numpy()]
 
         return l
 
-def preprocess_standard(text, keep_words=set()):
+def preprocess_standard(text, keep_words=set(), limit=5, downsample=True):
     """
     Standard preprocessing: filter out rare (<=5 occurences) words, downsample common words.
 
     Args:
         text (list): text as a list of strs
+        keep_words: (set): words that are kept in the vocabulary regardless of frequency
+        limit: (int): words with fewer occurences are discarded
+        downsample: whether to do downsampling of common words
 
     Returns:
         text, vocabulary: text as a list of strs, vocabulary as a set of strs
     """
     N = len(text)
-    text, counts = filter_rare_words(text, keep_words=keep_words)
-    text = downsample_common_words(text, counts)
+    text, counts = filter_rare_words(text, limit=limit, keep_words=keep_words)
+    if downsample:
+        text = downsample_common_words(text, counts)
 
     vocabulary = set(text)
     freqs = {wd: counts[wd] / N for wd in list(vocabulary)}
     return text, freqs
 
-def preprocess_partitioned(texts, labels, keep_words=set()):
+def preprocess_partitioned(texts, labels, keep_words=set(), limit=5, downsample=True):
     """
     Standard preprocessing for partitioned datasets: filter out rare (<=5 occurences) words, downsample common words.
 
     Args:
         texts (list): list of texts, each element of which is a list of strs
         labels (list): label associated with each 
+        keep_words: (set): words that are kept in the vocabulary regardless of frequency
+        limit: (int): words with fewer occurences are discarded
+        downsample: whether to do downsampling of common words
 
     Returns:
         text, vocabulary: text as a list of list of strs, vocabulary as a set of strs
     """
     assert len(texts) == len(labels), "Number of data partitions and labels must be equal"
     assert isinstance(texts[0], list), "Data should be provided as a list of lists"
     N = sum([len(t) for t in texts])
-    texts, counts = filter_rare_words(texts, keep_words=keep_words)
-    texts = [downsample_common_words(text, counts) for text in texts]
+    texts, counts = filter_rare_words(texts, limit=limit, keep_words=keep_words)
+    if downsample:
+        texts = [downsample_common_words(text, counts) for text in texts]
 
     def add_subscript(t, subscript):
         if not isinstance(t, tf.Tensor):
             t = tf.constant(t)
         t = t + f"_{subscript}"
         t = [wd.decode("utf-8") for wd in t.numpy()]
         return t
```

### Comparing `probabilistic_word_embeddings-1.2.0/probabilistic_word_embeddings/utils.py` & `probabilistic_word_embeddings-1.2.1/probabilistic_word_embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.2.0/setup.py` & `probabilistic_word_embeddings-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'progressbar2',
  'scikit-learn',
  'tensorflow-probability>=0.11,<0.12',
  'tensorflow>=2.2,<3.0']
 
 setup_kwargs = {
     'name': 'probabilistic-word-embeddings',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': 'Probabilistic Word Embeddings for Python',
     'long_description': 'None',
     'author': 'Your Name',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `probabilistic_word_embeddings-1.2.0/PKG-INFO` & `probabilistic_word_embeddings-1.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probabilistic-word-embeddings
-Version: 1.2.0
+Version: 1.2.1
 Summary: Probabilistic Word Embeddings for Python
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

