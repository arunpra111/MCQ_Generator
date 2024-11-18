
# MCQ Generator Using NLP

This project is designed to generate multiple-choice questions (MCQs) from a given text using various NLP techniques. The MCQ generation involves the following steps:

1. **Text Summarization**: A summarizer is used to condense the input text into a more concise form.
2. **Keyword Extraction**: Keywords are extracted from the summary of the text using the RAKE algorithm.
3. **Sentence Tokenization**: The summarized text is split into individual sentences.
4. **Mapping Sentences to Keywords**: Sentences are mapped to the extracted keywords.
5. **Distractor Generation**: Distractors (incorrect answers) are generated using WordNet synonyms.
6. **MCQ Creation**: MCQs are formed by replacing keywords in sentences with blanks (________), and the correct answer along with distractors are provided.

## How to Use

### Google Colab
You can run this project directly in Google Colab. Simply copy the provided code and paste it into a Colab notebook. It will automatically install the necessary dependencies and generate MCQs from your input text.

1. **Install the dependencies** using the following commands in a Colab cell:
    ```bash
    !pip install transformers
    !pip install torch
    !pip install rake-nltk
    !pip install nltk
    ```
2. **Paste the code** into a Colab cell.
3. **Input text**: Provide your own text in the `text` variable, or enter it interactively in the provided input section.
4. **Generate MCQs**: After running the code, the MCQs will be displayed in the output.