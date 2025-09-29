# 🌐 English-Hindi Translation Project

A simple project for processing English-Hindi datasets and evaluating Google Gemini's translation quality! 🚀

## 📁 What's Inside

```
task 1/
├── main1.ipynb              📊 Dataset processing
├── main2.ipynb              🤖 Translation with Gemini
├── train.xlsx               📋 Raw data from Hugging Face
├── output_dataset_1.xlsx    ✨ Clean processed data
└── translation_metrics.txt 📈 Evaluation results
```

## 🔥 Part 1: Dataset Processing (main1.ipynb)

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

## 🤖 Part 2: Translation Testing (main2.ipynb)

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

1. Run `main1.ipynb` first 📊
2. Check that `train.xlsx` is created ✅
3. Run `main2.ipynb` for translation testing 🤖
4. Check  results `train.xlsx` ! 📈

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