
# TP3: Understanding and Implementing Word Embeddings with Word2Vec

This project is part of the Machine Learning course of the Master's program in Artificial Intelligence, specifically under the Automatic Language Processing class. It aims to understand and implement word embeddings using the Word2Vec toolkit. Word embeddings are a type of word representation that allows words to be represented as vectors in a continuous vector space, capturing semantic and syntactic similarities among words.

## Overview

The main objective of this practical session is to explore the functionality of word embeddings through the Word2Vec toolkit. These embeddings are capable of capturing contextual, semantic, and syntactic nuances of words in real-valued vectors.

## Getting Started

### Prerequisites

- Python programming environment
- Gensim library for Word2Vec
- Access to the `text8` corpus
- Word2Vec and ConvertVec tools

### Setup

1. **Data Preparation**: Download the `text8` corpus, a pre-processed subset of Wikipedia text.

   ```
   wget http://mattmahoney.net/dc/text8.zip -O text8.gz
   gzip -d text8.gz -f
   ```

2. **Word2Vec Installation**: Clone and compile the Word2Vec toolkit.

   ```
   git clone https://github.com/tmikolov/word2vec
   cd word2vec
   make
   ```

3. **ConvertVec Installation**: Useful for converting binary Word2Vec models to text format.

   ```
   git clone https://github.com/marekrei/convertvec
   cd convertvec
   make
   ```

## Training Word2Vec Model

Train word embeddings on the `text8` corpus using the following command, which includes various parameters like vector size, window size, and more.

```
./word2vec -train text8 -output vectors400.bin -cbow 1 -size 400 -window 8 -negative 25 -hs 0 -sample 1e-4 -threads 20 -binary 1 -iter 15
```

## Understanding Word2Vec Options

The command line options for Word2Vec training control various aspects of the training process and model architecture, influencing the quality and characteristics of the resulting word embeddings.

## Exploring Semantic Similarities

One of the fascinating aspects of word embeddings is their ability to place semantically similar words close to each other in the vector space. This project includes examples of finding words closely related to a given set of words, such as "best," "football," "france," and "wine," as well as exploring the vectors for specific words like "hello."

## Analogy Tasks

Word embeddings can also solve word analogy tasks, showcasing the model's ability to capture relationships between words beyond simple similarity.

## Converting Binary Model to Text

To edit and view the vectors, the binary file `vectors400.bin` is converted to text format using ConvertVec.

```
./convertvec bin2txt vectors400.bin vectors400.txt
```

## Observations and Insights

The project offers insights into the semantic relationships captured by word vectors, discussing the results of closest word queries and analogy tasks, and highlighting the potential and limitations of the Word2Vec model.

## Contributions and Licensing

This project is open for contributions. The `text8` dataset is utilized for training purposes, and the project is intended for educational purposes under the guidance of Mickael Rouvier, as part of the Machine Learning and Automatic Language Processing curriculum.
