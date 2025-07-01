# DialoGPT Large: Dialogue Evaluation & Visualization

This project demonstrates how to evaluate and visualize the performance of Microsoft's `DialoGPT-large` conversational language model using a dataset sourced from Kaggle.

## 📌 Features

- Integration with KaggleHub to download datasets  
- Preprocessing and cleaning of dialogue data  
- Tokenization using Hugging Face's `transformers`  
- Perplexity computation to assess language model performance  
- Visualization tools:
  - Training loss graph
  - Token confidence heatmaps
  - Word clouds (optional)

## 🚀 Installation

Clone this repository and install dependencies:

```bash
git clone https://github.com/yourusername/dialoGPT-dialogue-eval.git
cd dialoGPT-dialogue-eval
pip install -r requirements.txt
```
Install additional dependencies inside a Jupyter/Colab notebook:

python
Copy
Edit
!pip install kagglehub transformers torch wordcloud matplotlib seaborn
📂 Dataset
You must upload your kaggle.json file to authenticate and access the dataset:

python
Copy
Edit
from google.colab import files
files.upload()  # Upload your kaggle.json
The dataset is automatically downloaded using:

python
Copy
Edit
import kagglehub
path = kagglehub.dataset_download("mathurinache/dialogptlarge")
🛠️ Usage
Clean and Tokenize Dialogue
python
Copy
Edit
cleaned = clean_text(raw_text)
tokens = tokenize_dialogues([cleaned])
Calculate Perplexity
python
Copy
Edit
ppl = calculate_perplexity(tokens)
print("Model Perplexity:", ppl)
Plot Loss Graph
python
Copy
Edit
plot_loss_graph([1.85, 1.72, 1.55, 1.42])  # Example values
Visualize Token Confidence
python
Copy
Edit
visualize_token_confidence("How are you doing today?")
🧰 Technologies Used
Python 3

Hugging Face Transformers

PyTorch

KaggleHub

Matplotlib & Seaborn

WordCloud (optional)

#🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.

#📄 License
This project is licensed under the MIT License.

#👤 Author
Your Name — [https://github.com/Deekshithpoleboina]
