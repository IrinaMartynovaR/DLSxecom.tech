# DLSxcom.tech

This project implements a multi-label text classification model using the `cointegrated/rubert-tiny2` BERT variant. The model processes customer reviews, cleans and translates associated tags into Russian, and trains a classifier to predict multiple labels.

## Installation

To set up the project on your local machine, follow these steps:

1. Clone the repository:
   git clone https://github.com/IrinaMartynovaR/DLSxcom.tech.git
2. Navigate to the project directory:
   cd DLSxcom.tech
3. Install the required dependencies:
   pip install -r requirements.txt
   
Usage

To run the project, ensure that you have a CSV file named train.csv in the root directory of your project. The CSV should contain the necessary columns for processing.

    Open a Jupyter Notebook or Python script and execute the code provided in bert_for_ecomtech.ipynb.

    The code performs the following steps:
        Imports necessary libraries and sets up configurations.
        Cleans and translates the tags.
        Prepares the data for training and validation.
        Initializes the tokenizer and encodes the text data.
        Defines the dataset class for text classification.
        Initializes the BERT model for multi-label classification.

Data Preparation

The input data should contain the following columns:

    text: The customer reviews.
    tags: Tags associated with each review.

Data Cleaning and Tag Translation

The tags are cleaned and translated from English to Russian using a predefined dictionary. The cleaned tags are combined with the original text to create a new feature called text_tags.

Model Training

The model is trained using the Trainer class from the transformers library. The dataset is split into training and validation sets, and the model is configured for multi-label classification.

