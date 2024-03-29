# Awesome-Papers

Awesome papers contrain list of papers that I go through over the time. Try to crate quick summary and key points from the papers for helping myself. If it helps others then it would be great. Papers are categorized based on domain of the papers

## NLP

### 19 July 2021
- **Paper:** [Deep Natural Language Processing for LinkedIn Search Systems](https://arxiv.org/pdf/2108.08252.pdf)
- **Domain:** `LinkedIn search system using DeepNLP`
- **Kye points:** In this paper, we introduce a comprehensive study of applying deep NLP techniques to five representative tasks in search engines. Through the model design and experiments of the five tasks, readers can find answers to three important questions: 

  - (1) When is deep NLP helpful/not helpful in search systems?
  - (2) How to address latency challenges?
  - (3) How to ensure model robustness?
  - `5 Search tasks`
    - Query Intent Prediction - Use `CNN with 128 filters`
    - Query Tagging - Use `Semi-markov conditional random field (SCRF)`
    - Query auto completion - Use `one layer LSTM with a 100 dimension hidden state`
    - Query Suggestion - Use `seq2seq mode contain 100 hidden size and 2 layers in LSTM`
    - Document Ranking - Use `xgboost`

![](./images/linkedin-search-system.png)

### 2 Jun 2021
- **Paper:** [mproving Named Entity Recognition by External Context Retrieving and Cooperative Learning](https://arxiv.org/pdf/2105.03654v2.pdf)
- **Domain:** `Name Entity Recognition`

### ACL 2020
- **Paper:** [Representation Learning for Information Extraction from Form-like Documents](https://research.google/pubs/pub49122/)
- **Discussion:** [Extracting Structured Data from Templatic Documents ](https://ai.googleblog.com/2020/06/extracting-structured-data-from.html)

### ACL 2020
- **Paper:** [TAPAS: Weakly Supervised Table Parsing via Pre-training](https://arxiv.org/abs/2004.02349) 
- **Discussion:** [Using Neural Networks to Find Answers in Tables ](https://ai.googleblog.com/2020/04/using-neural-networks-to-find-answers.html)

### 26 Aug 2017
 - **Paper:** [Neural Collaborative Filtering](https://arxiv.org/pdf/1708.05031.pdf)
 - **Domain:** `Recommender systems`, `Collaborative  Filtering`,  `Matrix Factorization`, `Implicit Feedback`
 - **Dataset:** `Movie Lens`
 - **Discussion:** [Introducing TensorFlow Recommenders ](https://blog.tensorflow.org/2020/09/introducing-tensorflow-recommenders.html)
 - **Key points:** Present a general framework named NCF, short for Neural network-based Collaborative Filtering. NCF is generic and can ex-press and generalize  matrix factorization under its frame-work. To supercharge NCF modelling with non-linearities,we propose to leverage a multi-layer perceptron to learn theuser–item  interaction  function. Extensive  experiments on two real-world datasets show significant improvements of ourproposed NCF framework over the state-of-the-art methods. Empirical evidence shows that using deeper layers of neuralnetworks offers better recommendation performance.

![](./images/neural_collaborative_filtering_framework.png)

Neural collaborative filtering framework

### 16 May 2016
 - **Paper:** [Large Scale Distributed Semi-Supervised Learning Using Streaming Approximation](https://arxiv.org/pdf/1512.01752.pdf)
 - **Domain:** `Graph based semi-supervisedlearning (SSL)`, `Knowledge graph, Graph neural netwrok`, `Chatbot`, `Conversation AI`
 - **Dataset:** `Freebase-Entity`, `Freebase-Relation`
 - **Discussion:** [On device machine intelegence for chat applications](https://ai.googleblog.com/2017/02/on-device-machine-intelligence.html)
 - **Key points:** Graph  augmentation strategy using unsupervised deep learning architectures that yields further significantquality gains for SSL in natural  language applications.
 
![](./images/conversation_ai_flow.png)

In top messages along with projections and corresponding replies, if available, are used in a machine learning framework to jointly learn a “message projection model”. (Bottom) The message projection model learns to associate replies with the projections of the corresponding incoming messages. For example, the model projects two different messages “Howdy, everything going well?” and “How’s it going buddy?” (bottom center) to nearby bit vectors and learns to map these to relevant replies (bottom right).

### 7 Apr 2016
- **Paper:** [Neural Architectures for Named Entity Recognition](https://arxiv.org/pdf/1603.01360.pdf)
- **Domain:** `Name Entity Recognition`, `PoS Tagger`, `LSTM-CRFL`, `Stack-LSTM`, `Structured Prediction`
- **Dataset:** `CoNLL-2002`, `CoNLL-2003`
- **Discussion:**
    - [Tagger](https://github.com/glample/tagger)
    - [Stack LSTM NER](https://github.com/clab/stack-lstm-ner)
    - [Spacy Name Entity Recognizer](https://www.youtube.com/watch?v=sqDHBH9IjRU&t=2902s)

![](./images/transition-based-ner-shift-reduce-perser.png)

In this paper, weintroduce two new neural architectures one based on bidirectional LSTMs and conditional random fields, and the other that constructs and labels segments using a `transition-based` approach inspired by `shift-reduce parsers`. Our models rely on two sources of information about words: character-based word representations learned from the supervised corpus and unsupervised word representations learned from unannotated corpora.  Our models obtain state-of-the-art performance in NER in four languages without resorting toany language-specific knowledge or resourcessuch as gazetteers

### 22 July 2015
 - **Paper:** [A Neural Conversational Model](https://arxiv.org/pdf/1506.05869.pdf)
 - **Domain:** `Chatbot`, `Conversation AI`
 - **Dataset:** `IT helpdesk troubleshooting`, `Open domain movie transcript`
 - **Discussion:** [Towards a Conversational Agent that Can Chat About Anything ](https://ai.googleblog.com/2020/01/towards-conversational-agent-that-can.html)
 - **Key points:** Our approach makes use of the sequence-to-sequence(seq2seq) framework.The model is based on a recurrent neural network whichreads the input sequence one token at a time, and predictsthe output sequence, also one token at a time. During train-ing, the true output sequence is given to the model, so learn-ing can be done by backpropagatio
 
![](./images/seq2seq_for_conversational_ai.png)
 
 The seq2seq framework for modeling conversations.


### 17 May 2019
 - **Paper:** [Gmail Smart Compose: Real-Time Assisted Writing](https://arxiv.org/pdf/1906.00080.pdf)
 - **Domain:** `Smart Compose`, `Language model`, `Assisted writing`
 - **Dataset:**  `8 billion English email message`
 - **Discussion:**
 - **Key points:** Present Smart Compose, a novel system for gener-ating interactive, real-time suggestions in Gmail that assists usersin writing mails by reducing repetitive typing.
 
![](./images/email_compose.png)
 
Smart email compose architecture


## Computer vision

### 22 Sep 2020
 - **Paper:** [PP-OCR: A Practical Ultra Lightweight OCR System](https://arxiv.org/pdf/2009.09941.pdf)
 - **Domain:** `Text detection`, `Direction classification`, `Text recognition`
 
 ### 15 Jun 2019
 -**Paper:** [Offline Handwritten Chinese Text Recognition with Convolutional Neural Networks](https://arxiv.org/ftp/arxiv/papers/2006/2006.15619.pdf)
 -**Code:** [Handwritten chinese ocr](https://github.com/intel/handwritten-chinese-ocr-samples)
 
 ### 
 - **Paper:** [LARGEBATCHTRAINING  OFCONVOLUTIONALNET-WORKS](https://arxiv.org/pdf/1708.03888.pdf)
 - **Domain:** `Techinical Report`, `Learge Batch Training`, `AlexNet`

## Speech

### 27 Aug 2019
- **Paper:** [Jasper: An End-to-End Convolutional Neural Acoustic Mode](https://arxiv.org/pdf/1904.03288.pdf)
- **Domain:** `speech  recognition, convolutional networks,time-delay neural networks`
- **Dataset:** `LibriSpeech`
- **Code:** [jasper-asr](https://github.com/stefanpantic/asr)
- **Kye points:** This paper makes the following contributions:
  1.  We present a computationally efficient end-to-end con-volutional neural network acoustic model.
  2.  We show ReLU and batch norm outperform other combi-nations for regularization and normalization, and resid-ual connections are necessary for training to   converge.
  3.  We introduceNovoGrad, a variant of the Adam opti-mizer with a smaller memory footprint.
  4.  We improve the SOTA WER on LibriSpeech test-clean.

### 04 April 2019
-**Paper:** [Very Deep Self-Attention Networks for End-to-End Speech Recognition](https://arxiv.org/pdf/1904.13377.pdf)
-**Domain:** `Transformer`, `Speech Recognition`

### 22 Oct 2020
- **Paper:** [wav2vec 2.0: A Framework for Self-SupervisedLearning of Speech Representations](https://arxiv.org/pdf/2006.11477.pdf)
