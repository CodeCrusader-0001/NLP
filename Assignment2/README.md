# IndicCorpV2 Hindi Word Tokenization and Analysis

This Google Colab notebook demonstrates the process of loading, tokenizing, and performing basic statistical analysis on a subset of the IndicCorpV2 Hindi dataset.

## Overview

The notebook performs the following steps:

1.  **Load Dataset**: Streams a subset of the IndicCorpV2 Hindi dataset (~100k tokens) using the `datasets` library.
2.  **Tokenization**:
    *   Splits the text into sentences based on common Hindi and English punctuation marks (।, ., ?, !).
    *   Tokenizes sentences into words, cleaning punctuation and keeping only words, numbers, URLs, emails, and dates.
3.  **Save Output**: Saves the cleaned, word-tokenized sentences to a text file (`tokenized_words.txt`).
4.  **Corpus Statistics**: Calculates and displays basic statistics about the tokenized corpus, including:
    *   Total sentences
    *   Total words
    *   Total characters
    *   Average sentence length
    *   Average word length
    *   Type/Token Ratio (TTR)

## Requirements

*   Google Colab environment
*   Libraries: `datasets`, `regex`

## Usage

1.  Open the notebook in Google Colab.
2.  Run the code cells sequentially.
3.  The output will display the progress, the generated statistics, and a sample of the tokenized sentences.
4.  The cleaned word-tokenized data will be saved to `tokenized_words.txt` in the Colab environment.

## Code Details

*   **Dataset Loading**: Uses `datasets.load_dataset` with `streaming=True` to efficiently handle a potentially large dataset.
*   **Sentence Tokenization**: Employs a regular expression to split text by sentence-ending punctuation.
*   **Word Tokenization**: Uses a comprehensive regex pattern to identify and extract desired tokens (words, numbers, URLs, etc.) while discarding punctuation.
*   **Statistics**: Standard Python list comprehensions and basic arithmetic are used to compute corpus metrics.

## Output File

The `tokenized_words.txt` file contains one sentence per line, with words separated by spaces. This file can be used for further natural language processing tasks.

## Author

[Your Name or Alias (Optional)]

## License

[Specify a License, e.g., MIT, Apache 2.0 (Optional)]
