# QoS Sentiment Analysis using BERT and DNN

This project applies Natural Language Processing (NLP) and Deep Learning to analyze user sentiment from benchmark data, simulating real-time Quality of Service (QoS) optimization for live video game streaming platforms like Twitch and YouTube Gaming.

## 📌 Objective

As live streaming grows, it faces issues like fluctuating network performance and unpredictable viewer engagement. This project simulates a data-driven approach using:

- 🧠 **Big Data Analytics**
- 💬 **BERT-based Sentiment Analysis**
- 🔍 **Deep Neural Networks (DNN)** for viewer satisfaction classification

This system aims to help platforms dynamically adjust QoS based on live feedback and viewer sentiment.

---

## 📁 Project Structure

QoS-Sentiment-Analysis/
│
├── data/
│ └── dataset.csv # Benchmark sentiment dataset
│
├── src/
│ ├── data_loader.py # Loads and splits dataset
│ ├── preprocess.py # Tokenizer setup (BERT)
│ ├── model.py # BERT + DNN model
│ └── train.py # Training pipeline
│
├── notebooks/
│ └── analysis.ipynb # EDA and model testing
│
├── requirements.txt # Project dependencies
├── README.md # Project overview
└── .gitignore # Files ignored by Git

---

## 📊 Dataset

- **Source**: [Text Emotion Dataset](https://github.com/dair-ai/emotion_dataset)
- **Content**: Over 20,000 labeled text entries with emotional sentiment
- **Used for**: Simulating real-time chat feedback

---

## 🚀 How to Run

### 🧪 Set up Environment

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/qos-sentiment-analysis.git
   cd qos-sentiment-analysis

2.Install dependencies:
pip install -r requirements.txt

3.Download and place the dataset:

Place text_emotion.csv inside data/ and rename it to dataset.csv
4.Run training:
python src/train.py

 Model Architecture
Pre-trained Model: bert-base-uncased (HuggingFace)

Classification Layer: Custom Deep Neural Network on top of BERT’s pooled output

Loss Function: Cross Entropy Loss

Optimizer: Adam

✅ Output
Text input → Emotion category (e.g., happy, sad, angry)

Prints training loss and final test accuracy

Enables downstream integration for real-time QoS decision-making

📈 Future Work
Integrate with real-time chat streams (Twitch API)

Auto-adjust stream resolution/latency based on sentiment

Deploy using Streamlit or Flask for demo


📚 NLP Project – 2025

📎 License
This project is part of an academic assignment and not licensed for commercial use.

