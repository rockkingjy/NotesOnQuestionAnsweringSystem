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
