## Overview

The notebook performs the following steps:

1.  **Task**: IndicCorpV2 Hindi Word Tokenization and Analysis.
2.  **Process**:
    *   **Load Dataset**: Streams a subset of the IndicCorpV2 Hindi dataset (~100k tokens) using the `datasets` library.
    *   **Tokenization**:
        *   Splits the text into sentences based on common Hindi and English punctuation marks (।, ., ?, !).
        *   Tokenizes sentences into words, cleaning punctuation and keeping only words, numbers, URLs, emails, and dates.
    *   **Save Output**: Saves the cleaned, word-tokenized sentences to a text file (`tokenized_words.txt`).
    *   **Corpus Statistics**: Calculates and displays basic statistics about the tokenized corpus, including:
        *   Total sentences
        *   Total words
        *   Total characters
        *   Average sentence length
        *   Average word length
        *   Type/Token Ratio (TTR)
