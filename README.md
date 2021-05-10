# NLP-Learning
Natural language processing (NLP) can be defined asthe automatic (orsemi-automatic) processing of human language.
The five phases of NLP involve lexical (structure) analysis, parsing, semantic analysis, discourse integration, and pragmatic analysis.

Some NLP applications
• spelling and grammar checking
• optical character recognition (OCR)
• screen readers for blind and partially sighted users

Some simple statistical techniques:
A corpus (corpora is the plural) is simply a body of text that has been collected for some purpose. A balanced corpus contains texts which represent different genres (newspapers, fiction, textbooks, parliamentary reports, cooking recipes, scientific papers etc).Distributed corpora are often annotated in some way: the most important type of annotation for NLP is part-of-speech tagging (POS tagging).
Corpora are needed in NLP for two reasons. Firstly, we have to evaluate algorithms on real language: corpora are required for this purpose for any style of NLP. Secondly, corpora provide the data source for many machine-learning approaches.

Prediction : The essential idea of prediction is that, given a sequence of words, we want to determine what’s most likely to come next. The main difficulty with using statistical
prediction models is in finding enough data: to be useful, the model really has to be trained on an individual speaker’s output, but of course very little of this is likely to be available. Prediction is important in estimation of entropy, including estimations of the entropy of English.Other applications for prediction include optical character recognition (OCR), spelling correction and text segmentation for languages such as Chinese, etc.

A bigram model assigns a probability to a word based on the previous word: i.e. P(wn|wn−1) where wn is the nth word in some string. 

Part of speech tagging
Prediction techniques can be used for word classes, rather than just individual words. One important application is to part-of-speech tagging (POS tagging), where the words in a corpus are associated with a tag indicating some syntactic information that applies to that particular use of the word.

 Stochastic POS tagging
One form of POS tagging applies the N-gram technique that we saw above, but in this case it applies to the POS tags rather than the individual wordsThe idea of stochastic POS tagging is that the tag can be assigned based on consideration of the lexical probability (how likely it is that the word has that tag), plus the sequence of prior tags. For a bigram model, we only look at a single previous tag. This is slightly more complicated than the word prediction case because we have to take into account both words and tags.

How to build an NLP pipeline
There are the following steps to build an NLP pipeline -
Step1: Sentence Segmentation
Sentence Segment is the first step for building the NLP pipeline. It breaks the paragraph into separate sentences.

Step2: Word Tokenization
Word Tokenizer is used to break the sentence into separate words or tokens.

Step3: Stemming
Stemming is used to normalize words into its base form or root form. For example, celebrates, celebrated and celebrating, all these words are originated with a single root word "celebrate." The big problem with stemming is that sometimes it produces the root word which may not have any meaning.

Step 4: Lemmatization
Lemmatization is quite similar to the Stamming. It is used to group different inflected forms of the word, called Lemma. The main difference between Stemming and lemmatization is that it produces the root word, which has a meaning.

Step 5: Identifying Stop Words
In English, there are a lot of words that appear very frequently like "is", "and", "the", and "a". NLP pipelines will flag these words as stop words. Stop words might be filtered out before doing any statistical analysis.

Step 6: Dependency Parsing
Dependency Parsing is used to find that how all the words in the sentence are related to each other.

Step 7: POS tags
POS stands for parts of speech, which includes Noun, verb, adverb, and Adjective. It indicates that how a word functions with its meaning as well as grammatically within the sentences. A word has one or more parts of speech based on the context in which it is used.

Step 8: Named Entity Recognition (NER)
Named Entity Recognition (NER) is the process of detecting the named entity such as person name, movie name, organization name, or location.

Step 9: Chunking
Chunking is used to collect the individual piece of information and grouping them into bigger pieces of sentences.
