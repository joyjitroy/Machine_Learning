# NLP Stock Sentiment Analysis: A Comparative Embedding-Based Model Report

This repository contains the complete implementation, datasets, and supplementary materials for the paper:

**“NLP Stock Sentiment Analysis: A Comparative Embedding-Based Approach”  
(Preprint submitted to arXiv, 2025)**  
Author: **Joyjit Roy**  
Email: **joyjit.roy@gmail.com**  
Zenodo DOI (Dataset + Documentation): **https://doi.org/10.5281/zenodo.17510735**  
Hugging Face Repository: **https://huggingface.co/joyjitroy/Stock_Market_News_Sentiment_Analysis**

---
## 📌 Project Overview

This project presents a reproducible NLP-based pipeline for classifying financial news sentiment and aggregating weekly sentiment trends. The system converts headline-level financial news into structured numerical indicators using embedding-based representations and a Gradient Boosting classifier.

Three embedding approaches were evaluated:

- **Word2Vec** (trained locally, 300-dimensional)  
- **GloVe** (pretrained, 100-dimensional)  
- **SentenceTransformer-based sentence embeddings** (384-dimensional)

Weekly text summaries were generated using **Mistral-7B-Instruct**, illustrating how sentiment outputs can support market commentary and analysis workflows.

The project includes:

✔ Full Jupyter Notebook  
✔ Public dataset (CSV via Zenodo)  
✔ Ready-to-publish arXiv paper  
✔ Weekly sentiment aggregation + LLM summarization  
✔ Model results (1 figure, 3 tables)

---
## 📂 Repository Structure

```plaintext
/
├── README.md
├── NLP_Stock_Sentiment_Analysis_Full_Code.ipynb
├── stock_news.csv                            
└── NLP Stock Sentiment Analysis - Model Report.pdf
```
---
## 📈 Key Features

- End-to-end NLP pipeline for financial sentiment  
- Word-level and sentence-level embeddings  
- Gradient Boosting classifier with hyperparameter tuning  
- Evaluation using accuracy, precision, recall, F1 score, and error rate  
- Temporal aggregation into weekly sentiment indicators  
- LLM-generated weekly financial summaries  
- Fully reproducible workflow  

---
## 🗂 Dataset

The dataset includes 349 headline-level financial news samples paired with:
- Date  
- Headline text  
- OHLCV market indicators  
- Sentiment labels (1, 0, -1)

Download from Zenodo:
👉 **https://doi.org/10.5281/zenodo.17510735**

---
## ⚙️ How to Run
1. Clone the repository:
```bash
git clone https://github.com/joyjitroy/NLP-Stock-Sentiment-Analysis
cd NLP-Stock-Sentiment-Analysis
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Open the notebook:
```bash
jupyter notebook NLP_Stock_Sentiment_Analysis_Full_Code.ipynb
```
---

## 📊 Model Performance Summary
The tuned **GloVe model** achieved the strongest validation performance:
- Accuracy: **0.714**  
- Precision: **0.758**  
- Recall: **0.714**  
- F1 Score: **0.694**  
- Error Rate: **0.286**
See **Table 3** in the paper for the full comparison.

---
## 🧠 Weekly Sentiment Summarization
After classification, headlines were aggregated weekly and summarized using:
- **Mistral-7B-Instruct** (no fine-tuning)  
- One summary per week (18 weeks)  
- Provides narrative insight into market patterns

---
## 📄 Citation
If you use this work, please cite the SSRN preprint:

```
Roy, Joyjit, NLP Stock Sentiment Analysis: A Comparative Embedding-Based Model Report (August 01, 2024). Available at SSRN: https://ssrn.com/abstract=5784922 or http://dx.doi.org/10.2139/ssrn.5784922
```
---
## 📬 Contact

**Email:** joyjit.roy.tech@gmail.com  
**LinkedIn:** https://www.linkedin.com/in/royjoyjit

