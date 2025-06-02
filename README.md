# Context-Aware Dialogue Generation Using Generative AI

## 📌 Overview

This project focuses on enhancing the naturalness and relevance of virtual assistant conversations using advanced generative AI techniques. It proposes a context-aware framework for dialogue generation, leveraging transformer-based models to produce coherent, contextually relevant responses in real time.

---

## 📂 Project Description

The notebook explores how generative models, particularly in the field of NLP, can improve dialogue generation by incorporating conversational context. The solution is aimed at virtual assistants, enabling them to maintain consistent and intelligent multi-turn conversations.

Key elements include:

- Context extraction and management
- Use of pretrained models like DialoGPT
- Sequence generation and evaluation
- Performance metrics and visualizations

> 🔍 Notebook: [`GAI____Project.ipynb`](./GAI____Project.ipynb)

---

## 🔧 Features

- ✅ Preprocessing and formatting of conversation datasets
- 🧠 Use of transformer-based generative models (e.g., GPT-2, DialoGPT-Large)
- 🧾 Context tracking and dialogue history management
- 📈 Evaluation metrics: BLEU, ROUGE, and Perplexity
- 📊 Visual analysis of model outputs
- 📥 Integration with KaggleHub for pretrained model downloads

---

## 🤖 Pretrained Model

This project uses a pretrained version of **DialoGPT-Large**, downloaded using KaggleHub:

```python
import kagglehub
path = kagglehub.dataset_download("mathurinache/dialogptlarge")
print("Path to dataset files:", path)


## 🛠️ Installation

To set up the project locally, follow these steps:

```bash
# Clone the repository
git clone https://github.com/Deekshithpoleboina/AIML-2024.git
cd AIML-2024

# (Optional) Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
