# 📰 News Topic Classifier Using BERT

A Natural Language Processing (NLP) project that fine-tunes the **BERT (bert-base-uncased)** transformer model to classify news headlines into four categories using the **AG News Dataset** from Hugging Face.

---

## 📌 Project Overview

This project demonstrates how to build a complete text classification pipeline using a pre-trained transformer model. Instead of training a language model from scratch, BERT is fine-tuned on the AG News dataset using the Hugging Face Transformers library.

The application can classify a news headline into one of the following categories:

- 🌍 World
- ⚽ Sports
- 💼 Business
- 💻 Sci/Tech

---

## 🚀 Features

- Fine-tuned **BERT (bert-base-uncased)** model
- AG News Dataset from Hugging Face
- Text tokenization using BERT Tokenizer
- Model training using Hugging Face Trainer API
- Evaluation using Accuracy and F1-Score
- Confusion Matrix visualization
- Save and reload trained model
- Live prediction using Gradio

---

## 📂 Dataset

**Dataset:** AG News

Source:
https://huggingface.co/datasets/ag_news

The dataset contains four news categories:

| Label | Category |
|-------|-----------|
| 0 | World |
| 1 | Sports |
| 2 | Business |
| 3 | Sci/Tech |

---

## 🛠 Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- Hugging Face Datasets
- Scikit-learn
- NumPy
- Pandas
- Matplotlib
- Gradio
- Jupyter Notebook

---

## 📁 Project Structure

```
News-Topic-Classifier-BERT/
│
├── notebook.ipynb
├── README.md
├── requirements.txt
│
├── saved_model/
│   ├── config.json
│   ├── model.safetensors
│   ├── tokenizer.json
│   ├── tokenizer_config.json
│   ├── special_tokens_map.json
│   ├── vocab.txt
│   └── labels.json
│

```

---

## ⚙ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/News-Topic-Classifier-BERT.git
```

Move into the project directory

```bash
cd News-Topic-Classifier-BERT
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶ Training

Run the Jupyter notebook to:

- Load AG News dataset
- Preprocess text
- Tokenize headlines
- Fine-tune BERT
- Evaluate the model
- Save the trained model

---

## 📊 Evaluation Metrics

The model is evaluated using:

- Accuracy
- Weighted F1 Score
- Classification Report
- Confusion Matrix

---

## 💾 Saved Model

After training, the following files are generated:

```
saved_model/
│
├── config.json
├── model.safetensors
├── tokenizer.json
├── tokenizer_config.json
├── special_tokens_map.json
├── vocab.txt
└── labels.json
```

These files are required to reload the trained model for inference.

---

## 🔮 Predicting New Headlines

Example:

Input

```
Apple launches its latest AI-powered processor.
```

Prediction

```
Sci/Tech
```

---

## 🌐 Gradio Deployment

Launch the application using:

```python
interface.launch()
```

Open the generated local URL in your browser and enter any news headline for live prediction.

---

## 📈 Machine Learning Workflow

```
Load Dataset
      │
      ▼
Text Preprocessing
      │
      ▼
Tokenization
      │
      ▼
Load Pretrained BERT
      │
      ▼
Fine-tune Model
      │
      ▼
Evaluate Model
      │
      ▼
Save Model
      │
      ▼
Load Saved Model
      │
      ▼
Predict New Headlines
```

---

## 🎯 Skills Demonstrated

- Natural Language Processing (NLP)
- Transformer Models
- Transfer Learning
- BERT Fine-Tuning
- Text Classification
- Hugging Face Transformers
- Model Evaluation
- Deep Learning with PyTorch
- Model Deployment with Gradio

---

## 📚 Future Improvements

- Support additional news categories
- Multi-language classification
- Hyperparameter optimization
- Deploy using Streamlit or FastAPI
- Docker containerization
- Cloud deployment

---

## 👨‍💻 Author

**Anas Ibrahim**

BS Computer Science

University of Central Punjab (UCP)

---

## 📄 License

This project is created for educational and learning purposes.
