# AI Detection of Gambling Promotion

This project aims to detect gambling-related promotional content using Artificial Intelligence approaches, including NLP models and Large Language Models (LLMs).

---

## 📌 Background
The rise of online gambling promotions has become a serious issue in digital platforms. Automated detection is needed to reduce harmful exposure and improve content moderation systems.

---

## 🎯 Objectives
- Classify text into gambling promotion or non-promotion
- Compare performance between:
  - IndoBERT (Transformer-based model)
  - GPT (zero-shot & few-shot)
- Evaluate models using standard metrics

---

## 📂 Project Structure

```
AI-Detection-Gambling-Promotion/
│
├── 📁 Dataset/              # Raw & cleaned datasets
├── 📁 GPT Model/            # GPT zero-shot & few-shot experiments
├── 📁 IndoBERT/             # Fine-tuned IndoBERT model & configs
├── 📁 Prediction Results/   # Model predictions & evaluation outputs
├── 📁 Preprocessing/        # Data cleaning & preprocessing scripts
│
├── 📄 .gitignore
└── 📄 README.md
```


---

## ⚙️ Methods

### 1. Preprocessing
- Text cleaning
- Normalization
- Tokenization

### 2. Models
- **IndoBERT**: Fine-tuned for classification
- **GPT**:
  - Zero-shot learning
  - Few-shot learning

### 3. Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score

---

## 📊 Results

### 🔹 GPT-based Approach

| Method     | Accuracy | Precision | Recall | F1 Score |
|------------|----------|----------|--------|----------|
| Zero-Shot  | 86.95%   | 94.99%   | 72.09% | 81.97%   |
| Few-Shot   | 90.91%   | 95.43%   | 81.83% | 88.11%   |

### 🔹 IndoBERT Model

| Model          | Accuracy | Precision | Recall | F1 Score |
|----------------|----------|----------|--------|----------|
| IndoBERT Base  | 99.41%   | 99.64%   | 98.93% | 99.28%   |

---

## 📈 Analysis

- The **few-shot GPT approach** shows a clear improvement over zero-shot, especially in recall and F1-score.
- The **IndoBERT model significantly outperforms GPT-based methods** across all evaluation metrics.
- This suggests that:
  - Fine-tuned transformer models (like IndoBERT) are highly effective for domain-specific classification tasks.
  - GPT models, while flexible, may require more context or fine-tuning to achieve comparable performance.
- The high performance of IndoBERT may also indicate:
  - Strong dataset quality
  - Potential overfitting (should be validated with additional test sets)

---

## ⚠️ Limitations

- GPT evaluation depends heavily on prompt design
- IndoBERT results may not generalize well without further validation
- Dataset scope is limited to specific gambling-related content

## 🚀 How to Run

1. Clone repository:
git clone https://github.com/Apexionn/AI-Detection-Gambling-Promotion.git

2. Open notebooks:
- Preprocessing.ipynb
- TrainSLM.ipynb
- PredictionSLM.ipynb

---

## 📌 Notes
- Large model files are excluded using `.gitignore`
- This project is intended for academic purposes

---

## 👤 Author
Lintang Anggowoyuono
