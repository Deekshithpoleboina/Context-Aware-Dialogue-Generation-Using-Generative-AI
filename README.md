# 💬 DialoGPT Large: Dialogue Evaluation & Visualization

This project demonstrates how to evaluate and visualize the performance of Microsoft's `DialoGPT-large` conversational language model using a dataset sourced from Kaggle.

---

## 📂 Dataset

- **Source**: [DialoGPT Dataset (KaggleHub)](https://www.kaggle.com/datasets/mathurinache/dialogptlarge)
- **Model Used**: microsoft/DialoGPT-large
- **Usage**: Token-level evaluation and response generation

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

- 🔄 Dataset download using KaggleHub  
- 🧽 Preprocessing and cleaning of dialogue data  
- 🧠 Tokenization using Hugging Face `transformers`  
- 📊 Perplexity calculation for evaluating model performance  
- 📈 Visual tools:
  - Loss graph over time
  - Token confidence visualization
  - Optional word cloud generation

---

## ⚙️ Methodology

1. **Setup**
   - Upload `kaggle.json` to authenticate KaggleHub
   - Download dataset from Kaggle using `kagglehub`

2. **Model & Tokenizer**
   - Load `microsoft/DialoGPT-large` from Hugging Face
   - Process text using the tokenizer

3. **Evaluation**
   - Compute perplexity over the test samples
   - Visualize training loss trends
   - Visualize token-level confidence scores

---

## 🧪 Usage

### 📦 Install Dependencies (Colab or Jupyter)

```python
!pip install kagglehub transformers torch wordcloud matplotlib seaborn
📁 Upload Dataset Key
python
Copy
Edit
from google.colab import files
files.upload()  # Upload your kaggle.json
⬇️ Download Dataset
python
Copy
Edit
import kagglehub
path = kagglehub.dataset_download("mathurinache/dialogptlarge")
🧼 Preprocess & Tokenize
python
Copy
Edit
cleaned = clean_text(raw_text)
tokens = tokenize_dialogues([cleaned])
📉 Evaluate Perplexity
python
Copy
Edit
ppl = calculate_perplexity(tokens)
print("Model Perplexity:", ppl)
📊 Visualize Loss and Confidence
python
Copy
Edit
plot_loss_graph([1.85, 1.72, 1.55, 1.42])
visualize_token_confidence("How are you doing today?")
📁 Project Structure
perl
Copy
Edit
📦 dialoGPT-dialogue-eval
├── dialoGPT_dialogue_eval.py       # Full source code
├── sample_dataset/                 # (Optional) Dialogue examples
├── README.md                       # Project documentation
├── requirements.txt                # Dependencies list
📉 Visualizations
Token-level confidence scores using softmax logits

Training loss vs. epoch

(Optional) Word cloud from dialogues

🚀 Future Enhancements
Integrate user-controlled conversation loops

Fine-tune DialoGPT with domain-specific data

Build interactive chatbot interface

Deploy with Streamlit or Gradio for live demos

👨‍💻 Author
Deekshith Poleboina
📍 GitHub: https://github.com/Deekshithpoleboina

📄 License
This project is licensed under the MIT License. See the LICENSE file for details.
