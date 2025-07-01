# 💬 DialoGPT Large: Dialogue Evaluation & Visualization

This project demonstrates how to evaluate and visualize the performance of Microsoft's `DialoGPT-large` conversational language model using a dataset sourced from Kaggle.

---

## 📂 Dataset

- **Source**: [DialoGPT Dataset (KaggleHub)](https://www.kaggle.com/datasets/mathurinache/dialogptlarge)
- **Model**: `microsoft/DialoGPT-large`
- **Task**: Evaluate and visualize response quality via token-level analysis

---

## 🛠️ Tools & Libraries

- Python 3  
- Hugging Face Transformers  
- PyTorch  
- KaggleHub  
- Matplotlib, Seaborn  
- WordCloud *(optional)*

---

## 📌 Features

- Dataset download from KaggleHub  
- Dialogue cleaning and preprocessing  
- Tokenization with Hugging Face  
- Perplexity computation  
- Visualization:
  - Training loss plot
  - Token confidence visualization
  - Optional word cloud

---

## ⚙️ Methodology

1. **Setup**
   - Upload `kaggle.json` to authenticate KaggleHub
   - Download dataset from Kaggle using `kagglehub`

2. **Model & Tokenizer**
   - Load `microsoft/DialoGPT-large` from Hugging Face
   - Process text using the tokenizer

3. **Evaluation**
   - Compute perplexity over test samples
   - Visualize token confidence and training loss

---

## 🚀 Usage

### 📦 Install Dependencies (Colab or Jupyter)

```bash
!pip install kagglehub transformers torch wordcloud matplotlib seaborn
```

### 🔐 Upload kaggle.json
```bash
from google.colab import files
files.upload()  # Upload your kaggle.json
```
