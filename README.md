
# Email Personalization Project

This project aims to personalize email responses by (1) scraping emails from a Gmail account and (2) fine-tuning the LLaMA 3 language model to generate emails that sound more like the user. 

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
  - [Email Collection and Cleaning](#email-collection-and-cleaning)
  - [Model Fine-Tuning](#model-fine-tuning)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Introduction

The goal of this project is to streamline and personalize email communication by leveraging machine learning. We achieve this by scraping emails from a Gmail account and fine-tuning a pre-trained LLaMA 3 language model to generate responses that mimic the user's writing style.

## Features

- **Email Scraping:** Collect emails from a Gmail account using the Gmail API.
- **Data Cleaning:** Clean and preprocess the collected email data.
- **Fine-Tuning:** Use QLoRA to fine-tune the LLaMA 3 model on the user's email data.
- **Email Generation:** Generate personalized email responses.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/email-personalization.git
   cd email-personalization
   ```

2. Create and activate a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up Gmail API credentials by following [this guide](https://developers.google.com/gmail/api/quickstart/python).

## Usage

### Email Collection and Cleaning

1. Navigate to the `email_collection_and_cleaning` directory and open the Jupyter notebook:
   ```bash
   cd email_collection_and_cleaning
   jupyter notebook email_collection_and_cleaning.ipynb
   ```

2. Follow the steps in the notebook to authenticate with Gmail, collect emails, and preprocess the data.

### Model Fine-Tuning

1. Navigate to the `llama_finetuning` directory and open the Jupyter notebook:
   ```bash
   cd ../llama_finetuning
   jupyter notebook llama_finetuning.ipynb
   ```

2. Follow the steps in the notebook to fine-tune the LLaMA 3 model using QLoRA on the preprocessed email data.

## Results

The fine-tuned LLaMA 3 model can generate personalized email responses that closely mimic the user's writing style. Example outputs and evaluation metrics can be found in the `results` directory.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to the developers of the LLaMA 3 model and the QLoRA method.
- Special thanks to the authors of the open-source libraries used in this project.
