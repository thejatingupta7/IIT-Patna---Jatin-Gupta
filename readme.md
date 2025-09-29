# 🌐 English-Hindi Translation Project

A simple project for processing English-Hindi datasets and evaluating Google Gemini's translation quality! 🚀

## 📁 What's Inside

```
task 1/
├── Assignment_1.ipynb              📊 Dataset processing
├── Assignment_2.ipynb              🤖 Translation with Gemini
├── Assignment_2.1.ipynb            🤖 Translation with Gemini (tuned prompt)
├── train.xlsx               📋 Raw data from Hugging Face
├── output_dataset_1.xlsx    ✨ Clean processed data
├── output_dataset_2.xlsx    ✨ English to Hindi (translated) text
├── output_dataset_2.1.xlsx    ✨ English to Hindi (translated) text (prompt tuned)
├── metrics_Assignment_2.txt  📈 Evaluation metrics 1 (Simple prompt)
└── metrics_Assignment_2.1.txt 📈 Evaluation metrics 2  (Prompt Tuned)
```

## 🔥 Assessment 1: English–Hindi Dataset Processing and Analysis (Assignment_1.ipynb)

### What it does:
- 📥 Loads English-Hindi dataset from Hugging Face
- 📊 Counts words in sentences
- 🔍 Filters out bad quality data
- 💾 Saves clean data to Excel

### The Process:
1. Load dataset 📂
2. Count words in English & Hindi sentences 🔢
3. Keep only good sentences (5-50 words) ✅
4. Remove sentences with huge word count differences ⚖️
5. Save clean dataset 💾

## 🤖  Assessment No. 2 – Translation with LLM (Assignment_2.ipynb)

### What it does:
- 🌟 Uses Google Gemini to translate 100 English sentences
- 📏 Compares with correct Hindi translations
- 📊 Gives scores: BLEU, CHRF, TER

### Simple Metrics:
- **BLEU**: How similar are the translations? 🎯
- **CHRF**: Character-level accuracy 🔤
- **TER**: How many errors? ❌

## ⚡ Quick Setup

### Install packages:
```bash
pip install datasets huggingface_hub pandas openpyxl google-generativeai sacrebleu
```

### Add your API keys:
```python
# Hugging Face
login(token="your_token_here")

# Google Gemini
client = genai.Client(api_key="your_gemini_key")
```

## 🚀 How to Run

1. Run `Assignment_1.ipynb` first 📊 to preprocess the text.
2. Check that `output_data_1.xlsx` is created ✅ (pre-processsed file)
3. Run `Assignment_2.ipynb` for translation testing 🤖 (Model translating)
4. Check translated text in `output_dataset_2.xlsx` ! 📈
5. Metric Score 1st run is in `metrics_Assignment_2.txt`!!  ✅  (SIMPLE PROMPT) --> LED TO OVER-EXPLANATION
6. Check translated text in `output_dataset_2.1.xlsx` ! 📈
7. Metric Score 2nd run is in `metrics_Assignment_2.1.txt`!!  ✅  (PROMPT TUNED) 

## 📈 Results

- **Clean Dataset**: Quality English-Hindi sentence pairs 
- **Translation Test**: 100 sentences translated by Gemini
- **Scores**: BLEU, CHRF, TER metrics saved to file

## ⚠️ Common Problems one can face

- **Can't access dataset?** 🔒 Check your Hugging Face token permissions
- **API errors?** 🚫 Make sure your Gemini API key works
- **Slow processing?** 🐌 Try smaller batches

## 👨‍🎓 Author

**Jatin Gupta** 
