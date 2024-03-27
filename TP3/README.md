
# TP3: Word Embeddings with Word2Vec

This project explores word embeddings using the Word2Vec model, demonstrating various aspects of training and utilizing word embeddings in natural language processing (NLP). It focuses on options for the word2vec program, cosine similarity calculation between word vectors, and finding words closest to a given set of words.

## Getting Started

### Prerequisites

Before running this project, ensure you have Python installed on your machine along with the necessary libraries, including `gensim` for Word2Vec modeling and `numpy` for handling vector operations.

### Installation

Clone this repository to your local machine to get started with the project:

```bash
git clone https://yourproject/repository.git
cd your-project-directory
```

Install the required Python dependencies:

```bash
pip install -r requirements.txt
```

### Usage

To train the Word2Vec model and explore word embeddings, follow the steps outlined in the `tp3.ipynb` Jupyter notebook. This notebook guides you through:

- Training a Word2Vec model with the specified parameters.
- Exploring the vector representation of words, such as the vector for 'hello'.
- Calculating the cosine similarity between two words.
- Finding words closest to a specified set of words, demonstrating semantic relationships captured by embeddings.

#### Command Line Interface (CLI)

Additionally, for direct command-line usage, refer to the example below:

```bash
python word2vec_options.py --train text8 --output vectors400.bin --size 400 --window 8
```

Replace `word2vec_options.py` with your script name if different.

## Contributing

We welcome contributions to improve this project. If you have suggestions or bug reports, please open an issue in the repository. For those who wish to contribute directly, please follow the standard fork-and-pull request workflow.

## Acknowledgments

- This project utilizes the `text8` corpus for training the Word2Vec model.
- Special thanks to the contributors of the `gensim` library for providing the tools necessary for working with word embeddings.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
