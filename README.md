
# Document Classification with BERT

Welcome to the Document Classification with BERT project! This project focuses on classifying documents into predefined categories using the BERT model.

## Introduction

Document classification involves categorizing documents into predefined categories. In this project, we leverage the power of BERT to perform document classification using a dataset of labeled documents.

## Dataset

For this project, we will use a custom dataset of labeled documents. You can create your own dataset and place it in the `data/document_classification_data.csv` file.

## Project Overview

### Prerequisites

- Python 3.6 or higher
- PyTorch
- Hugging Face Transformers
- Datasets
- Scikit-learn

### Installation

To set up the project, follow these steps:

```bash
# Clone this repository and navigate to the project directory:
git clone https://github.com/your-username/bert_document_classification.git
cd bert_document_classification

# Install the required packages:
pip install -r requirements.txt

# Ensure your data includes labeled documents. Place these files in the data/ directory.
# The data should be in a CSV file with two columns: text and label.

# To fine-tune the BERT model for document classification, run the following command:
python scripts/train.py --data_path data/document_classification_data.csv

# To evaluate the performance of the fine-tuned model, run:
python scripts/evaluate.py --model_path models/ --data_path data/document_classification_data.csv
