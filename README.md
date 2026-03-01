
---

# 📊 Financial Data Extraction with LLMs

## Overview
This project leverages **Large Language Models (LLMs)** to extract, process, and summarize information from financial documents (e.g., hearings, reports, filings). By combining PDF parsing libraries with transformer-based models, the pipeline automates the tedious task of reading and condensing long financial texts into structured insights.

---

## ✨ Features
- **PDF Parsing**: Uses `PyPDF2` and `pdfplumber` to extract raw text from financial documents.  
- **Text Cleaning & Preprocessing**: Regex and JSON utilities for structured formatting.  
- **LLM Summarization**: Transformer models (via Hugging Face `transformers` + `torch`) generate concise summaries of financial hearings.  
- **Configurable Workflow**: Modular design for easy adaptation to different document types.  
- **Reproducibility**: Environment pinned with `env.yml` and `requirements.txt` for consistent runs.

---

## 🛠️ Tech Stack
- **Python 3.12**  
- **Libraries**:  
  - `PyPDF2` – PDF text extraction  
  - `pdfplumber` – advanced PDF parsing  
  - `pdfminer.six` – low-level PDF text mining  
  - `transformers` – LLM integration  
  - `torch` – deep learning backend  
  - `json`, `re` – text structuring and regex cleaning  

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/Rusty-user365/Financial_Data_Extraction_LLM.git
cd Financial_Data_Extraction_LLM
```

### 2. Create environment
Using Conda:
```bash
conda env create -f env.yml
conda activate mlops_env
```

Or with pip:
```bash
pip install -r requirements.txt
```

### 3. Run the notebook
Open `LLM_PDF_data_Symmarisation.ipynb` in Jupyter/Colab and execute cells to parse PDFs and generate summaries.

---

## 📂 Project Structure
```
Financial_Data_Extraction_LLM/
│
├── LLM_PDF_data_Symmarisation.ipynb   # Main notebook for PDF summarization
├── requirements.txt                   # Python dependencies
├── env.yml                            # Conda environment definition
├── data/                              # Sample financial PDFs (not included in repo)
└── README.md                          # Project documentation
```

---

## 📈 Example Workflow
1. Upload a financial hearing PDF.  
2. Extract text using `pdfplumber`.  
3. Clean and preprocess text.  
4. Pass text chunks to an LLM for summarization.  
5. Output structured summaries in JSON format.

---

## 🔒 Reproducibility
- Environment pinned with Python 3.12 and exact library versions.  
- Random seeds set for deterministic behavior.  
- Dockerfile (optional) can be added for deployment in CI/CD pipelines.

---

## 🌐 Future Work
- Integrate **MongoDB Atlas** for storing extracted summaries.  
- Add **CI/CD pipelines on AWS** for automated deployment.  
- Extend to **multi-document summarization** and **financial Q&A bots**.  

---

## 🤝 Contributing
Pull requests are welcome! Please open an issue first to discuss major changes.

---

## 📜 License
This project is licensed under the MIT License.

---
