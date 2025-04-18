
# 📝 Text Summarization Project

This repository provides a Python implementation of **text summarization** techniques using state-of-the-art NLP libraries. The project includes both **extractive** and **abstractive** summarization approaches for automatically generating concise summaries of long text documents.

 ✨ Key Features:
- **📝 Extractive Summarization**: Extracts key sentences from the original text based on word frequency and importance.
- **🤖 Abstractive Summarization**: Utilizes a deep learning model (Facebook's BART) to generate a new, condensed summary that paraphrases the original content.

 🔧 Technologies Used:
- **spaCy**: Used for natural language processing, sentence tokenization, and feature extraction.
- **NLTK**: Provides tools for text preprocessing, such as tokenization.
- **Transformers**: Hugging Face's pre-trained BART model for generating abstractive summaries.

 ⚙️ Installation & Setup:
To run the project, install the required dependencies and download the necessary models using the following commands:

```bash
pip install spacy transformers nltk
python -m spacy download en_core_web_sm
python -c "import nltk; nltk.download('punkt')"
```

 🏗️ How It Works:
1. **🧹 Preprocessing**: Cleans the input text to remove HTML tags and unnecessary whitespaces.
2. **✂️ Extractive Summarization**: Uses **spaCy** to process the text and score sentences based on the frequency of non-stop words. It then selects the top `n` sentences to form a summary.
3. **🤖 Abstractive Summarization**: Leverages the **BART model** from Hugging Face to generate a human-like summary by rephrasing the original text into a shorter version.

 🚀 Usage:
Simply input your article into the script and call either the `extractive_summary()` or `abstractive_summary()` function to generate the summaries.

Example:
```python
article = "Your long article text here..."
cleaned_text = preprocess_text(article)

# Generate Extractive Summary
extractive_summary(cleaned_text)

# Generate Abstractive Summary
abstractive_summary(cleaned_text)
```

 🎯 Output:
- **🔹 Extractive Summary**: Selects the most relevant sentences from the text.
- **🔸 Abstractive Summary**: Creates a concise, paraphrased summary of the article.

 🤝 Contributing:
Feel free to fork this repository and submit pull requests. If you find any issues or have suggestions for improvements, please open an issue in the repository.

---

