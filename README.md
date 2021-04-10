# Authorwise-Text-Generation

One of the most important problems that the field of machine learning attempts to solve is the ability to reproduce human levels of intelligence
using the methods of mathematics, statistics, and computer science. An important facet of human intelligence is our ability to write long and
complex passages of text. The ability of an algorithm to do something similar would have major implications that would extend beyond the field of
computer science. 

In our project, we attempt to tackle this problem using various existing state-of-the-art algorithms as well as by designing our neural networks
and seeing how well they can capture the writing styles of well-known and prolific writers. We begin by giving a brief description of our dataset,
which consists of 1937 books and 645 different authors in the form of EPUB files. We describe the techniques we have used to prepare that dataset
by extracting text from the EPUB files and storing them in two different file formats. We analyze the training data using techniques such as
sentiment analysis and try to examine the extent to which our neural networks manage to replicate writing characteristics such as average sentence
length, frequent word usage, and an overall sentiment distribution and we present our findings accordingly. Moreover, we also use the state-of-the
art algorithms that currently exist to generate text after fine-tuning it to the style of that particular author. We finally built a user interface
that allows the user to automatically generate text by themselves. 

We experimented with the corpora of 10 different authors using state-of-the art algorithms such as LSTM and GPT-2. For our LSTM implementations, we
used both existing implementations such as textgenrnn as well as 10 different custom built neural networks, one for each author. Our first step was
to analyse the author’s corpus and to assign a mean compound sentiment score to each sentence in the corpus, as well as to calculate an overall
mean compound sentiment score for each author. We then trained 10 different neural networks and experimented with parameters including but not
limited to batch size, minimum word frequency, width of the neural network in terms of number of neurons, depth of the neural network in terms of
number of layers, dropout values as well as dropout layers, different optimizers as well as different word counts and diversity techniques. For
each author, we took diversity values ranging from 0.3 to 1.0 and we assigned each generated sentence a compound sentiment score as well as an
overall mean compound sentiment score for each body of generated text. We then compare the results of these experiments and present our findings.
We also conducted a general analysis that consisted of measuring metrics such as overlap of most frequent words, average sentence length and word
clouds across training text and generated text.
