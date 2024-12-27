# Classification of Urdu News Articles

This repository is a showcase portfolio project demonstrating the implementation of three machine learning models and a web scraping workflow for classifying Urdu news articles into predefined categories: Entertainment, Business, Sports, Science-Technology, and International.

With 1139 preprocessed articles, Neural Networks achieved 97.8% accuracy, outperforming Logistic Regression and Naive Bayes (~95.6%). Features were extracted via Bag of Words. Future plans include using advanced NLP techniques and expanding the dataset.

This is to demonstrate manually made machine learning models and their accuracy in predicting the correct categories.


## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Models](#models)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Urdu is a morphologically rich language, and classifying Urdu text requires handling unique linguistic complexities. This project demonstrates the application of machine learning techniques to classify Urdu news articles. The implementation includes:

- A scraping notebook to collect data from news websites.
- Three machine learning models implemented in Jupyter notebooks.
- A small dataset of Urdu news articles.

## Project Structure

The repository is organized as follows:

```
.
├── data
│   ├── urdu_articles.csv  # Dataset containing Urdu news articles
│   └── notebooks
│       ├── logistic_regression.ipynb  # Logistic Regression model
│       ├── multinomial_bayes.ipynb   # Multinomial Naive Bayes model
│       ├── neural_network.ipynb      # Neural Network model
│       └── scraper.ipynb             # Web scraping implementation
├── LICENSE
└── README.md
```

## Dataset

The dataset consists of Urdu news articles categorized into five categories:
- Entertainment
- Business
- Sports
- Science-Technology
- International

The data is stored in `data/urdu_articles.csv`. It includes preprocessed text data ready for training and evaluation.

## Models

### Multinomial Naive Bayes
- Utilizes bigram features for text classification.
- Implements Lidstone Smoothing for improved performance.

### Logistic Regression
- Implements a One-vs-All approach for multi-class classification.
- Optimized using Cross-Entropy Loss.

### Neural Network
- Architecture includes a single hidden layer with 256 neurons and ReLU activation.
- Trained using Adam optimizer and Cross-Entropy Loss.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/urdu-news-classification.git
   ```
2. Navigate to the project directory:
   ```bash
   cd urdu-news-classification
   ```
3. Run the notebooks:
   - Open `scraper.ipynb` to scrape Urdu news articles.
   - Use `logistic_regression.ipynb`, `multinomial_bayes.ipynb`, or `neural_network.ipynb` to explore model implementations.

## Contributing

Contributions are welcome! If you have improvements or suggestions, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

