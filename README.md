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
### ⬇️ Download Dataset
```bash
import kagglehub
path = kagglehub.dataset_download("mathurinache/dialogptlarge")
```
### 🧼 Preprocess & Tokenize
```bash
cleaned = clean_text(raw_text)
tokens = tokenize_dialogues([cleaned])
```
### 📉 Compute Perplexity
```bash
ppl = calculate_perplexity(tokens)
print("Model Perplexity:", ppl)
```
### 📊 Visualize Loss & Confidence
```bash
plot_loss_graph([1.85, 1.72, 1.55, 1.42])
visualize_token_confidence("How are you doing today?")
```
---
## 📁 Project Structure
```bash
📦 dialoGPT-dialogue-eval
├── dialoGPT_dialogue_eval.py       # Full source code
├── sample_dataset/                 # (Optional) Dialogue examples
├── README.md                       # Project documentation
├── requirements.txt                # Dependencies list
```
---
## 📉 Visualizations
- Training loss vs. epoch
- Token-level confidence (via softmax logits)
- Optional word cloud from dialogue data
---

## 🚀 Future Improvements
- Add user-controlled interactive loops
- Fine-tune DialoGPT on custom datasets
- Build and deploy chatbot using Streamlit or Gradio
- Add evaluation metrics like BLEU or ROUGE
---

## 👨‍💻 Author

**Deekshith**
GitHub:[https://github.com/Deekshithpoleboina](https://github.com/Deekshithpoleboina)
---
## 📄 License
This project is licensed under the MIT License. See the `LICENSE` file for details.


