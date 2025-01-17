# Telegram Data Processing and NER Labeling

## Objective

This project aims to preprocess Telegram data, label entities using Named Entity Recognition (NER) with spaCy, and achieve entity labeling for both English and Amharic text. The tasks are divided into two main steps: preprocessing data and labeling entities in the data.

## Setup

### Prerequisites

Ensure you have the following libraries installed:

- telethon
- python-dotenv
- pandas
- nest-asyncio
- spacy

You can install these libraries using the `requirements.txt` file.

### Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/your-repository.git
    cd your-repository
    ```

2. **Create a virtual environment (optional but recommended):**

    ```bash
    python -m venv env
    source env/bin/activate  # For Unix/macOS
    env\Scripts\activate  # For Windows
    ```

3. **Install the required packages:**

    ```bash
    pip install -r requirements.txt
    ```

4. **Download the spaCy English model:**

    ```bash
    python -m spacy download en_core_web_sm
    ```

## Project Structure

- `preprocessed_telegram_data.csv`: CSV file containing preprocessed Telegram data.
- `task1.ipynb`: Jupyter notebook for preprocessing Telegram data.
- `label_dataset_CoNLL.ipynb`: Jupyter notebook for NER entity labeling.
- `requirements.txt`: List of required Python packages.

## Usage

### Step 1: Preprocess Telegram Data

1. **Open the `task1.ipynb` notebook:**

    ```bash
    jupyter notebook task1.ipynb
    ```

2. **Execute the cells to preprocess Telegram data:**

    This notebook includes steps to preprocess the raw Telegram data and save it as `preprocessed_telegram_data.csv`.

### Step 2: Entity Labeling with spaCy

1. **Open the `label_dataset_CoNLL.ipynb` notebook:**

    ```bash
    jupyter notebook task2.ipynb
    ```

2. **Execute the cells to label entities:**

    This notebook processes the `preprocessed_telegram_data.csv` file, uses the spaCy model to label entities, and saves the labeled data in CoNLL format.


