# Comparing `tmp/tweetnlp-0.4.3.tar.gz` & `tmp/tweetnlp-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweetnlp-0.4.3.tar", last modified: Tue Apr 18 17:07:34 2023, max compression
+gzip compressed data, was "tweetnlp-0.4.4.tar", last modified: Wed Jun 14 20:16:19 2023, max compression
```

## Comparing `tweetnlp-0.4.3.tar` & `tweetnlp-0.4.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.936249 tweetnlp-0.4.3/
--rw-r--r--   0 asahi      (501) staff       (20)     1066 2022-05-24 10:28:20.000000 tweetnlp-0.4.3/LICENSE
--rw-r--r--   0 asahi      (501) staff       (20)    37239 2023-04-18 17:07:34.936549 tweetnlp-0.4.3/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)    36536 2023-04-18 17:07:13.000000 tweetnlp-0.4.3/README.md
--rw-r--r--   0 asahi      (501) staff       (20)       79 2023-04-18 17:07:34.937342 tweetnlp-0.4.3/setup.cfg
--rw-r--r--   0 asahi      (501) staff       (20)     1626 2023-04-18 16:55:23.000000 tweetnlp-0.4.3/setup.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.919638 tweetnlp-0.4.3/tweetnlp/
--rw-r--r--   0 asahi      (501) staff       (20)      537 2022-11-30 22:45:03.000000 tweetnlp-0.4.3/tweetnlp/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     3699 2022-12-04 19:32:28.000000 tweetnlp-0.4.3/tweetnlp/loader.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.922871 tweetnlp-0.4.3/tweetnlp/mlm/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-24 12:37:45.000000 tweetnlp-0.4.3/tweetnlp/mlm/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     4095 2022-11-28 13:37:18.000000 tweetnlp-0.4.3/tweetnlp/mlm/model.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.926859 tweetnlp-0.4.3/tweetnlp/ner/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-22 15:10:27.000000 tweetnlp-0.4.3/tweetnlp/ner/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)    28930 2022-11-26 19:43:35.000000 tweetnlp-0.4.3/tweetnlp/ner/allennlp_crf.py
--rw-r--r--   0 asahi      (501) staff       (20)      878 2022-11-30 22:45:03.000000 tweetnlp-0.4.3/tweetnlp/ner/dataset.py
--rw-r--r--   0 asahi      (501) staff       (20)     7056 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/ner/model.py
--rw-r--r--   0 asahi      (501) staff       (20)        6 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/ner/trainer.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.928380 tweetnlp-0.4.3/tweetnlp/question_answer_generation/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/question_answer_generation/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)      626 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/question_answer_generation/dataset.py
--rw-r--r--   0 asahi      (501) staff       (20)     2861 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/question_answer_generation/model.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.930590 tweetnlp-0.4.3/tweetnlp/question_answering/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/question_answering/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)      598 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/question_answering/dataset.py
--rw-r--r--   0 asahi      (501) staff       (20)     1651 2022-12-04 19:13:00.000000 tweetnlp-0.4.3/tweetnlp/question_answering/model.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.931831 tweetnlp-0.4.3/tweetnlp/sentence_embedding/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-24 12:34:58.000000 tweetnlp-0.4.3/tweetnlp/sentence_embedding/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     1874 2022-11-28 13:42:40.000000 tweetnlp-0.4.3/tweetnlp/sentence_embedding/model.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.935444 tweetnlp-0.4.3/tweetnlp/text_classification/
--rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-23 17:46:06.000000 tweetnlp-0.4.3/tweetnlp/text_classification/__init__.py
--rw-r--r--   0 asahi      (501) staff       (20)     2435 2022-11-30 22:45:03.000000 tweetnlp-0.4.3/tweetnlp/text_classification/dataset.py
--rw-r--r--   0 asahi      (501) staff       (20)    10261 2023-04-18 16:58:10.000000 tweetnlp-0.4.3/tweetnlp/text_classification/model.py
--rw-r--r--   0 asahi      (501) staff       (20)     5051 2022-12-02 18:24:51.000000 tweetnlp-0.4.3/tweetnlp/text_classification/readme_template.py
--rw-r--r--   0 asahi      (501) staff       (20)    15101 2022-12-02 18:24:51.000000 tweetnlp-0.4.3/tweetnlp/text_classification/trainer.py
--rw-r--r--   0 asahi      (501) staff       (20)     3986 2022-11-30 22:45:03.000000 tweetnlp-0.4.3/tweetnlp/util.py
-drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-04-18 17:07:34.922433 tweetnlp-0.4.3/tweetnlp.egg-info/
--rw-r--r--   0 asahi      (501) staff       (20)    37239 2023-04-18 17:07:34.000000 tweetnlp-0.4.3/tweetnlp.egg-info/PKG-INFO
--rw-r--r--   0 asahi      (501) staff       (20)      998 2023-04-18 17:07:34.000000 tweetnlp-0.4.3/tweetnlp.egg-info/SOURCES.txt
--rw-r--r--   0 asahi      (501) staff       (20)        1 2023-04-18 17:07:34.000000 tweetnlp-0.4.3/tweetnlp.egg-info/dependency_links.txt
--rw-r--r--   0 asahi      (501) staff       (20)       20 2023-04-18 17:07:34.000000 tweetnlp-0.4.3/tweetnlp.egg-info/entry_points.txt
--rw-r--r--   0 asahi      (501) staff       (20)      112 2023-04-18 17:07:34.000000 tweetnlp-0.4.3/tweetnlp.egg-info/requires.txt
--rw-r--r--   0 asahi      (501) staff       (20)        9 2023-04-18 17:07:34.000000 tweetnlp-0.4.3/tweetnlp.egg-info/top_level.txt
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-14 20:16:19.149029 tweetnlp-0.4.4/
+-rw-r--r--   0 asahi      (501) staff       (20)     1066 2022-05-24 10:28:20.000000 tweetnlp-0.4.4/LICENSE
+-rw-r--r--   0 asahi      (501) staff       (20)    37096 2023-06-14 20:16:19.149305 tweetnlp-0.4.4/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)    36393 2023-06-01 12:11:15.000000 tweetnlp-0.4.4/README.md
+-rw-r--r--   0 asahi      (501) staff       (20)       79 2023-06-14 20:16:19.150015 tweetnlp-0.4.4/setup.cfg
+-rw-r--r--   0 asahi      (501) staff       (20)     1626 2023-06-14 20:15:30.000000 tweetnlp-0.4.4/setup.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-14 20:16:19.132928 tweetnlp-0.4.4/tweetnlp/
+-rw-r--r--   0 asahi      (501) staff       (20)      537 2022-11-30 22:45:03.000000 tweetnlp-0.4.4/tweetnlp/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     3699 2022-12-04 19:32:28.000000 tweetnlp-0.4.4/tweetnlp/loader.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-14 20:16:19.137331 tweetnlp-0.4.4/tweetnlp/mlm/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-24 12:37:45.000000 tweetnlp-0.4.4/tweetnlp/mlm/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     4416 2023-06-14 20:14:43.000000 tweetnlp-0.4.4/tweetnlp/mlm/model.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-14 20:16:19.140620 tweetnlp-0.4.4/tweetnlp/ner/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-22 15:10:27.000000 tweetnlp-0.4.4/tweetnlp/ner/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)    28930 2022-11-26 19:43:35.000000 tweetnlp-0.4.4/tweetnlp/ner/allennlp_crf.py
+-rw-r--r--   0 asahi      (501) staff       (20)      878 2022-11-30 22:45:03.000000 tweetnlp-0.4.4/tweetnlp/ner/dataset.py
+-rw-r--r--   0 asahi      (501) staff       (20)     7377 2023-06-14 20:14:49.000000 tweetnlp-0.4.4/tweetnlp/ner/model.py
+-rw-r--r--   0 asahi      (501) staff       (20)        6 2022-12-04 19:13:00.000000 tweetnlp-0.4.4/tweetnlp/ner/trainer.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-14 20:16:19.142530 tweetnlp-0.4.4/tweetnlp/question_answer_generation/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2022-12-04 19:13:00.000000 tweetnlp-0.4.4/tweetnlp/question_answer_generation/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)      626 2022-12-04 19:13:00.000000 tweetnlp-0.4.4/tweetnlp/question_answer_generation/dataset.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2861 2022-12-04 19:13:00.000000 tweetnlp-0.4.4/tweetnlp/question_answer_generation/model.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-14 20:16:19.144351 tweetnlp-0.4.4/tweetnlp/question_answering/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2022-12-04 19:13:00.000000 tweetnlp-0.4.4/tweetnlp/question_answering/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)      598 2022-12-04 19:13:00.000000 tweetnlp-0.4.4/tweetnlp/question_answering/dataset.py
+-rw-r--r--   0 asahi      (501) staff       (20)     1651 2022-12-04 19:13:00.000000 tweetnlp-0.4.4/tweetnlp/question_answering/model.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-14 20:16:19.145159 tweetnlp-0.4.4/tweetnlp/sentence_embedding/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-24 12:34:58.000000 tweetnlp-0.4.4/tweetnlp/sentence_embedding/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     1874 2022-11-28 13:42:40.000000 tweetnlp-0.4.4/tweetnlp/sentence_embedding/model.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-14 20:16:19.148611 tweetnlp-0.4.4/tweetnlp/text_classification/
+-rw-r--r--   0 asahi      (501) staff       (20)        0 2022-05-23 17:46:06.000000 tweetnlp-0.4.4/tweetnlp/text_classification/__init__.py
+-rw-r--r--   0 asahi      (501) staff       (20)     2435 2022-11-30 22:45:03.000000 tweetnlp-0.4.4/tweetnlp/text_classification/dataset.py
+-rw-r--r--   0 asahi      (501) staff       (20)    10582 2023-06-14 20:14:34.000000 tweetnlp-0.4.4/tweetnlp/text_classification/model.py
+-rw-r--r--   0 asahi      (501) staff       (20)     5051 2022-12-02 18:24:51.000000 tweetnlp-0.4.4/tweetnlp/text_classification/readme_template.py
+-rw-r--r--   0 asahi      (501) staff       (20)    15101 2023-06-01 15:22:17.000000 tweetnlp-0.4.4/tweetnlp/text_classification/trainer.py
+-rw-r--r--   0 asahi      (501) staff       (20)     3986 2022-11-30 22:45:03.000000 tweetnlp-0.4.4/tweetnlp/util.py
+drwxr-xr-x   0 asahi      (501) staff       (20)        0 2023-06-14 20:16:19.136656 tweetnlp-0.4.4/tweetnlp.egg-info/
+-rw-r--r--   0 asahi      (501) staff       (20)    37096 2023-06-14 20:16:19.000000 tweetnlp-0.4.4/tweetnlp.egg-info/PKG-INFO
+-rw-r--r--   0 asahi      (501) staff       (20)      998 2023-06-14 20:16:19.000000 tweetnlp-0.4.4/tweetnlp.egg-info/SOURCES.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        1 2023-06-14 20:16:19.000000 tweetnlp-0.4.4/tweetnlp.egg-info/dependency_links.txt
+-rw-r--r--   0 asahi      (501) staff       (20)       20 2023-06-14 20:16:19.000000 tweetnlp-0.4.4/tweetnlp.egg-info/entry_points.txt
+-rw-r--r--   0 asahi      (501) staff       (20)      112 2023-06-14 20:16:19.000000 tweetnlp-0.4.4/tweetnlp.egg-info/requires.txt
+-rw-r--r--   0 asahi      (501) staff       (20)        9 2023-06-14 20:16:19.000000 tweetnlp-0.4.4/tweetnlp.egg-info/top_level.txt
```

### Comparing `tweetnlp-0.4.3/LICENSE` & `tweetnlp-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.3/PKG-INFO` & `tweetnlp-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tweetnlp
-Version: 0.4.3
+Version: 0.4.4
 Summary: NLP library for Twitter.
 Home-page: https://github.com/cardiffnlp/tweetnlp
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT
-Download-URL: https://github.com/cardiffnlp/tweetnlp/archive/0.4.3.tar.gz
+Download-URL: https://github.com/cardiffnlp/tweetnlp/archive/0.4.4.tar.gz
 Keywords: tweet,nlp,language-model
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
@@ -21,19 +21,19 @@
 
 [![license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://github.com/asahi417/tweetnlp/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/tweetnlp.svg)](https://badge.fury.io/py/tweetnlp)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tweetnlp.svg)](https://pypi.python.org/pypi/tweetnlp/)
 [![PyPI status](https://img.shields.io/pypi/status/tweetnlp.svg)](https://pypi.python.org/pypi/tweetnlp/)
 
 # TweetNLP
-TweetNLP for all the NLP enthusiasts working on Twitter! 
+TweetNLP for all the NLP enthusiasts working on Twitter and social media in general! 
 The python library `tweetnlp` provides a collection of useful tools to analyze/understand tweets such as sentiment analysis,
-emoji prediction, and named-entity recognition, powered by state-of-the-art language modeling trained on tweets.
+emoji prediction, and named-entity recognition, powered by state-of-the-art language modeling specialized on social media.
 
-***News (September 2022):*** Our paper presenting TweetNLP, "TweetNLP: Cutting-Edge Natural Language Processing for Social Media", has been accepted as an EMNLP 2022 system demonstration!! Camera-ready version can be found [here](https://arxiv.org/abs/2206.14774).
+***News (December 2022):*** We presented a TweetNLP demo paper ("TweetNLP: Cutting-Edge Natural Language Processing for Social Media"), at EMNLP 2022. The final version can be found [here](https://aclanthology.org/2022.emnlp-demos.5/).
 
 
 Resources:
 - Quick Tour with Colab Notebook: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/104MtF9MXkDFimlJLr4SFBX0HjidLTfvp?usp=sharing)
 - Play with the TweetNLP Online Demo: [link](https://tweetnlp.org/demo/)
 - EMNLP 2022 paper: [link](https://arxiv.org/abs/2206.14774)
 
@@ -150,15 +150,15 @@
 model.irony('If you wanna look like a badass, have drama on social media', return_probability=True)
 >>> {'label': 'irony', 'probability': {'non_irony': 0.08390884101390839, 'irony': 0.9160911440849304}} 
 
 # GET DATASET
 dataset, label2id = tweetnlp.load_dataset('irony')
 ```
 
-- ***Hate Speech Detection***: The hate speech dataset consists of detecting whether a tweet is hateful towards women or immigrants. It is based on the Detection of Hate Speech task at SemEval 2019 (check the paper [here](https://arxiv.org/pdf/2010.12421.pdf)).
+- ***Hate Speech Detection***: The hate speech dataset consists of detecting whether a tweet is hateful towards women or immigrants. It is based on a suite of unified hate speech detection datasets.
 
 ```python
 import tweetnlp
 
 # MODEL
 model = tweetnlp.load_model('hate')  # Or `model = tweetnlp.Hate()` 
 model.hate('Whoever just unfollowed me you a bitch')  # Or `model.predict`
@@ -218,15 +218,15 @@
   '📸': 0.04188741743564606,
   '😜': 0.011156936176121235}}
 
 # GET DATASET
 dataset, label2id = tweetnlp.load_dataset('emoji')
 ```
 
-- ***Emotion Recognition***: Given a tweet, this task consists of associating it with its most appropriate emotion. As a reference dataset we use the SemEval 2018 task on Affect in Tweets, simplified to only four emotions used in TweetEval: anger, joy, sadness and optimism (check the paper [here](https://arxiv.org/pdf/2010.12421.pdf)).
+- ***Emotion Recognition***: Given a tweet, this task consists of associating it with its most appropriate emotion. As a reference dataset we use the SemEval 2018 task on Affect in Tweets (check the paper [here](https://arxiv.org/pdf/2010.12421.pdf)). The latest multi-label model includes eleven emotion types.
 
 ```python
 import tweetnlp
 
 # MULTI-LABEL MODEL 
 model = tweetnlp.load_model('emotion')  # Or `model = tweetnlp.Emotion()` 
 model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.')  # Or `model.predict`
@@ -525,16 +525,14 @@
 
 For more details, please read the accompanying [TweetNLP's reference paper](https://arxiv.org/pdf/2206.14774.pdf). If you use TweetNLP in your research, please use the following `bib` entry to cite the reference paper:
 
 ```
 @inproceedings{camacho-collados-etal-2022-tweetnlp,
     title={{T}weet{NLP}: {C}utting-{E}dge {N}atural {L}anguage {P}rocessing for {S}ocial {M}edia},
     author={Camacho-Collados, Jose and Rezaee, Kiamehr and Riahi, Talayeh and Ushio, Asahi and Loureiro, Daniel and Antypas, Dimosthenis and Boisson, Joanne and Espinosa-Anke, Luis and Liu, Fangyu and Mart{\'\i}nez-C{\'a}mara, Eugenio and others},
-    author = "Ushio, Asahi  and
-      Camacho-Collados, Jose",
     booktitle = "Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing: System Demonstrations",
     month = nov,
     year = "2022",
     address = "Abu Dhabi, U.A.E.",
     publisher = "Association for Computational Linguistics",
 }
 ```
```

### Comparing `tweetnlp-0.4.3/README.md` & `tweetnlp-0.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [![license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://github.com/asahi417/tweetnlp/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/tweetnlp.svg)](https://badge.fury.io/py/tweetnlp)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tweetnlp.svg)](https://pypi.python.org/pypi/tweetnlp/)
 [![PyPI status](https://img.shields.io/pypi/status/tweetnlp.svg)](https://pypi.python.org/pypi/tweetnlp/)
 
 # TweetNLP
-TweetNLP for all the NLP enthusiasts working on Twitter! 
+TweetNLP for all the NLP enthusiasts working on Twitter and social media in general! 
 The python library `tweetnlp` provides a collection of useful tools to analyze/understand tweets such as sentiment analysis,
-emoji prediction, and named-entity recognition, powered by state-of-the-art language modeling trained on tweets.
+emoji prediction, and named-entity recognition, powered by state-of-the-art language modeling specialized on social media.
 
-***News (September 2022):*** Our paper presenting TweetNLP, "TweetNLP: Cutting-Edge Natural Language Processing for Social Media", has been accepted as an EMNLP 2022 system demonstration!! Camera-ready version can be found [here](https://arxiv.org/abs/2206.14774).
+***News (December 2022):*** We presented a TweetNLP demo paper ("TweetNLP: Cutting-Edge Natural Language Processing for Social Media"), at EMNLP 2022. The final version can be found [here](https://aclanthology.org/2022.emnlp-demos.5/).
 
 
 Resources:
 - Quick Tour with Colab Notebook: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/104MtF9MXkDFimlJLr4SFBX0HjidLTfvp?usp=sharing)
 - Play with the TweetNLP Online Demo: [link](https://tweetnlp.org/demo/)
 - EMNLP 2022 paper: [link](https://arxiv.org/abs/2206.14774)
 
@@ -129,15 +129,15 @@
 model.irony('If you wanna look like a badass, have drama on social media', return_probability=True)
 >>> {'label': 'irony', 'probability': {'non_irony': 0.08390884101390839, 'irony': 0.9160911440849304}} 
 
 # GET DATASET
 dataset, label2id = tweetnlp.load_dataset('irony')
 ```
 
-- ***Hate Speech Detection***: The hate speech dataset consists of detecting whether a tweet is hateful towards women or immigrants. It is based on the Detection of Hate Speech task at SemEval 2019 (check the paper [here](https://arxiv.org/pdf/2010.12421.pdf)).
+- ***Hate Speech Detection***: The hate speech dataset consists of detecting whether a tweet is hateful towards women or immigrants. It is based on a suite of unified hate speech detection datasets.
 
 ```python
 import tweetnlp
 
 # MODEL
 model = tweetnlp.load_model('hate')  # Or `model = tweetnlp.Hate()` 
 model.hate('Whoever just unfollowed me you a bitch')  # Or `model.predict`
@@ -197,15 +197,15 @@
   '📸': 0.04188741743564606,
   '😜': 0.011156936176121235}}
 
 # GET DATASET
 dataset, label2id = tweetnlp.load_dataset('emoji')
 ```
 
-- ***Emotion Recognition***: Given a tweet, this task consists of associating it with its most appropriate emotion. As a reference dataset we use the SemEval 2018 task on Affect in Tweets, simplified to only four emotions used in TweetEval: anger, joy, sadness and optimism (check the paper [here](https://arxiv.org/pdf/2010.12421.pdf)).
+- ***Emotion Recognition***: Given a tweet, this task consists of associating it with its most appropriate emotion. As a reference dataset we use the SemEval 2018 task on Affect in Tweets (check the paper [here](https://arxiv.org/pdf/2010.12421.pdf)). The latest multi-label model includes eleven emotion types.
 
 ```python
 import tweetnlp
 
 # MULTI-LABEL MODEL 
 model = tweetnlp.load_model('emotion')  # Or `model = tweetnlp.Emotion()` 
 model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.')  # Or `model.predict`
@@ -504,16 +504,14 @@
 
 For more details, please read the accompanying [TweetNLP's reference paper](https://arxiv.org/pdf/2206.14774.pdf). If you use TweetNLP in your research, please use the following `bib` entry to cite the reference paper:
 
 ```
 @inproceedings{camacho-collados-etal-2022-tweetnlp,
     title={{T}weet{NLP}: {C}utting-{E}dge {N}atural {L}anguage {P}rocessing for {S}ocial {M}edia},
     author={Camacho-Collados, Jose and Rezaee, Kiamehr and Riahi, Talayeh and Ushio, Asahi and Loureiro, Daniel and Antypas, Dimosthenis and Boisson, Joanne and Espinosa-Anke, Luis and Liu, Fangyu and Mart{\'\i}nez-C{\'a}mara, Eugenio and others},
-    author = "Ushio, Asahi  and
-      Camacho-Collados, Jose",
     booktitle = "Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing: System Demonstrations",
     month = nov,
     year = "2022",
     address = "Abu Dhabi, U.A.E.",
     publisher = "Association for Computational Linguistics",
 }
 ```
```

### Comparing `tweetnlp-0.4.3/setup.py` & `tweetnlp-0.4.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding="utf-8") as f:
     readme = f.read()
 
-version = '0.4.3'
+version = '0.4.4'
 setup(
     name='tweetnlp',
     packages=find_packages(exclude=["assets", "tests"]),
     version=version,
     license='MIT',
     description='NLP library for Twitter.',
     url='https://github.com/cardiffnlp/tweetnlp',
```

### Comparing `tweetnlp-0.4.3/tweetnlp/__init__.py` & `tweetnlp-0.4.4/tweetnlp/__init__.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.3/tweetnlp/loader.py` & `tweetnlp-0.4.4/tweetnlp/loader.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.3/tweetnlp/mlm/model.py` & `tweetnlp-0.4.4/tweetnlp/mlm/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,16 +12,22 @@
 class LanguageModel:
 
     def __init__(self, model_name: str = None, max_length: int = 128, use_auth_token: bool = False):
         model_name = DEFAULT_MLM_MODEL if model_name is None else model_name
         self.config, self.tokenizer, self.model = load_model(
             model_name, task='masked_language_model', use_auth_token=use_auth_token)
         self.max_length = max_length
-        # GPU setup
-        self.device = 'cuda' if torch.cuda.device_count() > 0 else 'cpu'
+        # GPU setup (https://github.com/cardiffnlp/tweetnlp/issues/15)
+        if torch.cuda.is_available() and torch.cuda.device_count() > 0:
+            self.device = torch.device('cuda')
+        elif hasattr(torch.backends, "mps") and torch.backends.mps.is_available() and torch.backends.mps.is_built():
+            self.device = torch.device("mps")
+        else:
+            self.device = torch.device('cpu')
+
         self.parallel = torch.cuda.device_count() > 1
         if self.parallel:
             self.model = torch.nn.DataParallel(self.model)
         self.model.to(self.device)
         logging.debug(f'{torch.cuda.device_count()} GPUs are in use')
         self.mask_prediction = self.predict  # function alias
         self.model.eval()
```

### Comparing `tweetnlp-0.4.3/tweetnlp/ner/allennlp_crf.py` & `tweetnlp-0.4.4/tweetnlp/ner/allennlp_crf.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.3/tweetnlp/ner/dataset.py` & `tweetnlp-0.4.4/tweetnlp/ner/dataset.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.3/tweetnlp/ner/model.py` & `tweetnlp-0.4.4/tweetnlp/ner/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,22 @@
                 num_tags=len(self.model.config.id2label),
                 constraints=allowed_transitions(constraint_type="BIO", labels=self.model.config.id2label)
             )
             self.crf_layer.load_state_dict(
                 {k: torch.FloatTensor(v) for k, v in self.model.config.crf_state_dict.items()}
             )
 
-        # GPU setup
-        self.device = 'cuda' if torch.cuda.device_count() > 0 else 'cpu'
+        # GPU setup (https://github.com/cardiffnlp/tweetnlp/issues/15)
+        if torch.cuda.is_available() and torch.cuda.device_count() > 0:
+            self.device = torch.device('cuda')
+        elif hasattr(torch.backends, "mps") and torch.backends.mps.is_available() and torch.backends.mps.is_built():
+            self.device = torch.device("mps")
+        else:
+            self.device = torch.device('cpu')
+
         self.parallel = torch.cuda.device_count() > 1
         if self.parallel:
             self.model = torch.nn.DataParallel(self.model)
             if self.crf_layer is not None:
                 self.crf_layer = torch.nn.DataParallel(self.crf_layer)
         self.model.to(self.device)
         if self.crf_layer is not None:
```

### Comparing `tweetnlp-0.4.3/tweetnlp/question_answer_generation/dataset.py` & `tweetnlp-0.4.4/tweetnlp/question_answer_generation/dataset.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.3/tweetnlp/question_answer_generation/model.py` & `tweetnlp-0.4.4/tweetnlp/question_answer_generation/model.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.3/tweetnlp/question_answering/dataset.py` & `tweetnlp-0.4.4/tweetnlp/question_answering/dataset.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.3/tweetnlp/question_answering/model.py` & `tweetnlp-0.4.4/tweetnlp/question_answering/model.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.3/tweetnlp/sentence_embedding/model.py` & `tweetnlp-0.4.4/tweetnlp/sentence_embedding/model.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.3/tweetnlp/text_classification/dataset.py` & `tweetnlp-0.4.4/tweetnlp/text_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.3/tweetnlp/text_classification/model.py` & `tweetnlp-0.4.4/tweetnlp/text_classification/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,16 +68,22 @@
             assert model_name is not None, "model_name is required"
             logging.debug(f'loading {model_name}')
             self.config, self.tokenizer, self.model = load_model(
                 model_name, task='sequence_classification', use_auth_token=use_auth_token)
         self.max_length = max_length
         self.multi_label = multi_label
         self.id_to_label = {str(v): k for k, v in self.config.label2id.items()}
-        # GPU setup
-        self.device = 'cuda' if torch.cuda.device_count() > 0 else 'cpu'
+        # GPU setup (https://github.com/cardiffnlp/tweetnlp/issues/15)
+        if torch.cuda.is_available() and torch.cuda.device_count() > 0:
+            self.device = torch.device('cuda')
+        elif hasattr(torch.backends, "mps") and torch.backends.mps.is_available() and torch.backends.mps.is_built():
+            self.device = torch.device("mps")
+        else:
+            self.device = torch.device('cpu')
+
         self.parallel = torch.cuda.device_count() > 1
         if self.parallel:
             self.model = torch.nn.DataParallel(self.model)
         self.model.to(self.device)
         logging.debug(f'{torch.cuda.device_count()} GPUs are in use')
 
         self.model.eval()
```

### Comparing `tweetnlp-0.4.3/tweetnlp/text_classification/readme_template.py` & `tweetnlp-0.4.4/tweetnlp/text_classification/readme_template.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.3/tweetnlp/text_classification/trainer.py` & `tweetnlp-0.4.4/tweetnlp/text_classification/trainer.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.3/tweetnlp/util.py` & `tweetnlp-0.4.4/tweetnlp/util.py`

 * *Files identical despite different names*

### Comparing `tweetnlp-0.4.3/tweetnlp.egg-info/PKG-INFO` & `tweetnlp-0.4.4/tweetnlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tweetnlp
-Version: 0.4.3
+Version: 0.4.4
 Summary: NLP library for Twitter.
 Home-page: https://github.com/cardiffnlp/tweetnlp
 Author: Asahi Ushio
 Author-email: asahi1992ushio@gmail.com
 License: MIT
-Download-URL: https://github.com/cardiffnlp/tweetnlp/archive/0.4.3.tar.gz
+Download-URL: https://github.com/cardiffnlp/tweetnlp/archive/0.4.4.tar.gz
 Keywords: tweet,nlp,language-model
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
@@ -21,19 +21,19 @@
 
 [![license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://github.com/asahi417/tweetnlp/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/tweetnlp.svg)](https://badge.fury.io/py/tweetnlp)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tweetnlp.svg)](https://pypi.python.org/pypi/tweetnlp/)
 [![PyPI status](https://img.shields.io/pypi/status/tweetnlp.svg)](https://pypi.python.org/pypi/tweetnlp/)
 
 # TweetNLP
-TweetNLP for all the NLP enthusiasts working on Twitter! 
+TweetNLP for all the NLP enthusiasts working on Twitter and social media in general! 
 The python library `tweetnlp` provides a collection of useful tools to analyze/understand tweets such as sentiment analysis,
-emoji prediction, and named-entity recognition, powered by state-of-the-art language modeling trained on tweets.
+emoji prediction, and named-entity recognition, powered by state-of-the-art language modeling specialized on social media.
 
-***News (September 2022):*** Our paper presenting TweetNLP, "TweetNLP: Cutting-Edge Natural Language Processing for Social Media", has been accepted as an EMNLP 2022 system demonstration!! Camera-ready version can be found [here](https://arxiv.org/abs/2206.14774).
+***News (December 2022):*** We presented a TweetNLP demo paper ("TweetNLP: Cutting-Edge Natural Language Processing for Social Media"), at EMNLP 2022. The final version can be found [here](https://aclanthology.org/2022.emnlp-demos.5/).
 
 
 Resources:
 - Quick Tour with Colab Notebook: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/104MtF9MXkDFimlJLr4SFBX0HjidLTfvp?usp=sharing)
 - Play with the TweetNLP Online Demo: [link](https://tweetnlp.org/demo/)
 - EMNLP 2022 paper: [link](https://arxiv.org/abs/2206.14774)
 
@@ -150,15 +150,15 @@
 model.irony('If you wanna look like a badass, have drama on social media', return_probability=True)
 >>> {'label': 'irony', 'probability': {'non_irony': 0.08390884101390839, 'irony': 0.9160911440849304}} 
 
 # GET DATASET
 dataset, label2id = tweetnlp.load_dataset('irony')
 ```
 
-- ***Hate Speech Detection***: The hate speech dataset consists of detecting whether a tweet is hateful towards women or immigrants. It is based on the Detection of Hate Speech task at SemEval 2019 (check the paper [here](https://arxiv.org/pdf/2010.12421.pdf)).
+- ***Hate Speech Detection***: The hate speech dataset consists of detecting whether a tweet is hateful towards women or immigrants. It is based on a suite of unified hate speech detection datasets.
 
 ```python
 import tweetnlp
 
 # MODEL
 model = tweetnlp.load_model('hate')  # Or `model = tweetnlp.Hate()` 
 model.hate('Whoever just unfollowed me you a bitch')  # Or `model.predict`
@@ -218,15 +218,15 @@
   '📸': 0.04188741743564606,
   '😜': 0.011156936176121235}}
 
 # GET DATASET
 dataset, label2id = tweetnlp.load_dataset('emoji')
 ```
 
-- ***Emotion Recognition***: Given a tweet, this task consists of associating it with its most appropriate emotion. As a reference dataset we use the SemEval 2018 task on Affect in Tweets, simplified to only four emotions used in TweetEval: anger, joy, sadness and optimism (check the paper [here](https://arxiv.org/pdf/2010.12421.pdf)).
+- ***Emotion Recognition***: Given a tweet, this task consists of associating it with its most appropriate emotion. As a reference dataset we use the SemEval 2018 task on Affect in Tweets (check the paper [here](https://arxiv.org/pdf/2010.12421.pdf)). The latest multi-label model includes eleven emotion types.
 
 ```python
 import tweetnlp
 
 # MULTI-LABEL MODEL 
 model = tweetnlp.load_model('emotion')  # Or `model = tweetnlp.Emotion()` 
 model.emotion('I love swimming for the same reason I love meditating...the feeling of weightlessness.')  # Or `model.predict`
@@ -525,16 +525,14 @@
 
 For more details, please read the accompanying [TweetNLP's reference paper](https://arxiv.org/pdf/2206.14774.pdf). If you use TweetNLP in your research, please use the following `bib` entry to cite the reference paper:
 
 ```
 @inproceedings{camacho-collados-etal-2022-tweetnlp,
     title={{T}weet{NLP}: {C}utting-{E}dge {N}atural {L}anguage {P}rocessing for {S}ocial {M}edia},
     author={Camacho-Collados, Jose and Rezaee, Kiamehr and Riahi, Talayeh and Ushio, Asahi and Loureiro, Daniel and Antypas, Dimosthenis and Boisson, Joanne and Espinosa-Anke, Luis and Liu, Fangyu and Mart{\'\i}nez-C{\'a}mara, Eugenio and others},
-    author = "Ushio, Asahi  and
-      Camacho-Collados, Jose",
     booktitle = "Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing: System Demonstrations",
     month = nov,
     year = "2022",
     address = "Abu Dhabi, U.A.E.",
     publisher = "Association for Computational Linguistics",
 }
 ```
```

### Comparing `tweetnlp-0.4.3/tweetnlp.egg-info/SOURCES.txt` & `tweetnlp-0.4.4/tweetnlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

