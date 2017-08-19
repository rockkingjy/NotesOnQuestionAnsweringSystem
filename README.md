# QuestionAnsweringSystemNotes
Some readings and notes of Question Answering System

Blogs and papers:

[[ACL](http://aclanthology.info)]

[[ACL Wiki](https://aclweb.org/aclwiki/Main_Page)]

[[刘康：基于深度学习的知识库问答研究进展](http://dataunion.org/29765.html)]

[[刘挺：人机对话技术的进展](http://scholarsupdate.hi2net.com/news.asp?NewsID=22708)]

[[Speech and Language Processing Dan Jurafsky](https://web.stanford.edu/~jurafsky/slp3/)]

[[NLP Lecture Slides from the Stanford Coursera course by Dan Jurafsky](https://web.stanford.edu/~jurafsky/NLPCourseraSlides.html)]

[[State of the art deep learning model for question answering](https://einstein.ai/research/state-of-the-art-deep-learning-model-for-question-answering)]

Datasets:

[[The leaderboard for the Stanford Question Answering Task](https://rajpurkar.github.io/SQuAD-explorer/)]

[[WebQuestions QA Benchmarking Dataset](https://github.com/brmson/dataset-factoid-webquestions)]

[[Datasets for Natural Language Processing](https://github.com/karthikncode/nlp-datasets#question-answering)]

[[Natural Language Understanding benchmark](https://github.com/snipsco/nlu-benchmark)]

[[QALD](https://qald.sebastianwalter.org/index.php?x=benchmark&q=home)]

中文Dataset：[[WebQA](http://idl.baidu.com/WebQA.html)]

Others:

[[NLP Job](http://www.nlpjob.com)]



--------
root@9b1bc77570ec:/home/DrQA# python prepro.py
08/19/2017 02:36:52 start data preparing...
08/19/2017 02:37:29 glove loaded.
08/19/2017 02:37:31 json data flattened.
08/19/2017 02:38:10 got intial tokens.
08/19/2017 02:38:23 drop 1320 inconsistent samples.
08/19/2017 02:38:23 answer pointer generated.
08/19/2017 02:42:45 tokens generated
08/19/2017 02:42:48 vocab coverage 91058/111467 | OOV occurrence 128308/14696898 (0.8730%)
08/19/2017 02:43:17 Found 56 POS tags.
08/19/2017 02:43:17 Found 19 entity tags: ['', 'ORG', 'DATE', 'PERSON', 'GPE', 'CARDINAL', 'NORP', 'LOC', 'WORK_OF_ART', 'PERCENT', 'EVENT', 'ORDINAL', 'MONEY', 'FAC', 'QUANTITY', 'LAW', 'TIME', 'LANGUAGE', 'PRODUCT']
08/19/2017 02:43:18 vocab built.
08/19/2017 02:44:02 got embedding matrix.
08/19/2017 02:44:11 saved to disk.

root@9b1bc77570ec:/home/DrQA# python train.py -e 20 -bs 32
08/19/2017 02:49:17 [program starts.]
08/19/2017 02:49:41 [Data loaded.]
08/19/2017 02:49:43 Epoch 1
08/19/2017 02:50:02 updates[     1] train loss[9.96538] remaining[14:01:18]
08/19/2017 02:50:30 updates[     4] train loss[9.31764] remaining[8:46:36]
08/19/2017 02:51:06 updates[     7] train loss[9.09595] remaining[8:51:32]
08/19/2017 02:51:39 updates[    10] train loss[8.99515] remaining[8:40:19]
08/19/2017 02:52:06 updates[    13] train loss[8.94023] remaining[8:12:28]
08/19/2017 02:52:41 updates[    16] train loss[8.86766] remaining[8:18:07]
08/19/2017 02:53:11 updates[    19] train loss[8.82763] remaining[8:08:02]
08/19/2017 02:53:37 updates[    22] train loss[8.74514] remaining[7:54:30]
08/19/2017 02:54:27 updates[    25] train loss[8.68598] remaining[8:25:24]
08/19/2017 02:54:57 updates[    28] train loss[8.64067] remaining[8:19:42]
08/19/2017 02:55:37 updates[    31] train loss[8.59011] remaining[8:27:03]
08/19/2017 02:56:04 updates[    34] train loss[8.53125] remaining[8:17:52]
08/19/2017 02:56:32 updates[    37] train loss[8.46768] remaining[8:10:28]
08/19/2017 02:57:00 updates[    40] train loss[8.44093] remaining[8:03:55]
08/19/2017 02:57:29 updates[    43] train loss[8.37998] remaining[7:59:00]
08/19/2017 02:57:53 updates[    46] train loss[8.34190] remaining[7:50:47]
08/19/2017 02:58:16 updates[    49] train loss[8.28205] remaining[7:42:28]
08/19/2017 02:58:40 updates[    52] train loss[8.22280] remaining[7:35:21]
08/19/2017 02:59:02 updates[    55] train loss[8.18218] remaining[7:27:22]
08/19/2017 02:59:26 updates[    58] train loss[8.14917] remaining[7:22:11]
08/19/2017 02:59:55 updates[    61] train loss[8.10092] remaining[7:20:49]
08/19/2017 03:00:18 updates[    64] train loss[8.05965] remaining[7:15:46]
08/19/2017 03:00:37 updates[    67] train loss[8.02944] remaining[7:08:07]
08/19/2017 03:01:20 updates[    70] train loss[8.00127] remaining[7:15:46]
08/19/2017 03:01:43 updates[    73] train loss[7.97268] remaining[7:11:30]
08/19/2017 03:02:06 updates[    76] train loss[7.93888] remaining[7:07:14]



