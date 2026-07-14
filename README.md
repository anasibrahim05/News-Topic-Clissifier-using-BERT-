# 📰 News Topic Classifier Using BERT

A Natural Language Processing (NLP) project that fine-tunes the **BERT (bert-base-uncased)** transformer model to classify news headlines into topic categories using the **AG News Dataset** from Hugging Face.

---

## 📌 Project Overview

This project demonstrates how to build a complete NLP text classification pipeline using a pre-trained BERT model. The model is fine-tuned on the AG News dataset to automatically classify news headlines into one of four categories.

### News Categories

- 🌍 World
- ⚽ Sports
- 💼 Business
- 💻 Sci/Tech

---

## 🚀 Features

- Fine-tuned BERT (bert-base-uncased)
- AG News Dataset from Hugging Face
- Text preprocessing and tokenization
- Transfer learning using Hugging Face Transformers
- Model evaluation using Accuracy and Weighted F1-Score
- Confusion Matrix and Classification Report
- Interactive prediction interface using Gradio
- Save and reload trained models

---

## 📂 Dataset

**Dataset:** AG News

https://huggingface.co/datasets/ag_news

Dataset Statistics:

- Training Samples: **120,000**
- Testing Samples: **7,600**
- Classes: **4**

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
├── News_Topic_Classifier.ipynb
├── app.py
├── README.md
├── requirements.txt
│
├── saved_model/
│   ├── config.json
│   ├── tokenizer.json
│   ├── tokenizer_config.json
│   ├── special_tokens_map.json
│   ├── vocab.txt
│   └── labels.json
│
└
```

---

## ⚙ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/News-Topic-Classifier-BERT.git
```

Move into the project

```bash
cd News-Topic-Classifier-BERT
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶ Model Training

The notebook performs the complete training pipeline:

1. Load the AG News dataset
2. Explore the dataset
3. Preprocess text
4. Tokenize news headlines using the BERT tokenizer
5. Fine-tune the pretrained BERT model
6. Evaluate the model
7. Save the trained model and tokenizer

---

## 📊 Evaluation

The model is evaluated using:

- Accuracy
- Weighted F1-Score
- Classification Report
- Confusion Matrix

---

## 💾 Saved Model

After training, the following files are generated:

```
saved_model/
├── config.json
├── tokenizer.json
├── tokenizer_config.json
├── special_tokens_map.json
├── vocab.txt
└── labels.json
```

> **Note**
>
> The trained model weights (`model.safetensors`) are **not included** in this repository because they exceed GitHub's file size limit.
>
> To generate the trained model, simply run the training notebook. The notebook will automatically create the `model.safetensors` file after fine-tuning.

---

## 🔮 Example Prediction

**Input**

```
Apple unveils its latest AI-powered processor for laptops.
```

**Prediction**

```
Sci/Tech
```

---

## 🌐 Gradio Deployment

Run:

```python
interface.launch()
```

A local web interface will open in your browser where you can enter a news headline and receive the predicted topic.

---

## 🔄 Project Workflow

```
Load AG News Dataset
        │
        ▼
Data Exploration
        │
        ▼
Text Preprocessing
        │
        ▼
BERT Tokenization
        │
        ▼
Load Pretrained BERT
        │
        ▼
Fine-Tune Model
        │
        ▼
Model Evaluation
        │
        ▼
Save Model & Tokenizer
        │
        ▼
Load Saved Files
        │
        ▼
Predict New Headlines
```

---

## 📈 Skills Demonstrated

- Natural Language Processing (NLP)
- Transformer Models
- Transfer Learning
- BERT Fine-Tuning
- Text Classification
- Hugging Face Transformers
- Model Evaluation
- Deep Learning with PyTorch
- Model Deployment using Gradio

---

## 📌 Future Improvements

- Support additional news datasets
- Multi-language news classification
- Hyperparameter optimization
- Streamlit deployment
- FastAPI REST API
- Docker containerization
- Cloud deployment

---

## 👨‍💻 Author

**Anas Ibrahim**

BS Computer Science

University of Central Punjab (UCP)

GitHub: https://github.com/yourusername

---

## 📄 License

This project is released for educational and learning purposes.
