# NLP Medical RAG System

## 📚 Overview
The **Medical RAG System** is a hybrid **Retrieval-Augmented Generation (RAG)** system designed to enhance medical information retrieval and question answering. This system integrates traditional sparse retrieval techniques (BM25) with dense retrieval methods (FAISS) and utilizes advanced Large Language Models (LLMs) like **MedPaLM** to provide enriched context for medical queries. The system aims to improve search precision, reduce hallucinations, and enhance contextual relevance, particularly in the medical domain.

---

## 🚀 Key Features
- **Hybrid Retrieval System**: Combines sparse (BM25) and dense (FAISS) retrieval techniques.
- **Advanced LLM Integration**: Utilizes MedPaLM for generating high-quality, domain-specific answers.
- **Publicly Available Datasets**: Trained and evaluated using MedQA-USMLE, Medical Meadow, and PubMedQA datasets.
- **High Precision Retrieval**: Ensures relevant information is retrieved, contextualized, and presented accurately.
- **Enhanced Response Quality**: Reduces hallucinations and improves relevance in medical contexts.

---

## 📊 Datasets
The following publicly available datasets were used for training and evaluation:
1. [**MedQA-USMLE Dataset**](https://huggingface.co/datasets/GBaker/MedQA-USMLE-4-options) : Multiple-choice questions for medical reasoning and knowledge.
2. [**Medical Meadow Dataset**](https://huggingface.co/datasets/medalpaca/medical_meadow_wikidoc) : Contextual biomedical data for retrieval tasks.
3. [**PubMedQA Dataset**](https://pubmed.ncbi.nlm.nih.gov/) : Clinical questions and answers sourced from PubMed articles.

---

## 🛠️ Methodology
The system was developed and evaluated using four retrieval approaches:
1. **Lexical Matching (Baseline)**: Simple keyword-based matching.
2. **BioBERT Retrieval**: Semantic-based retrieval using BioBERT for dense vector representations.
3. **FAISS + BioBERT Hybrid**: Combines BioBERT embeddings with FAISS for fast nearest-neighbor search.
4. **BM25 + BioBERT Hybrid**: Combines BM25 for lexical matching with BioBERT for semantic refinement.

---

## 📈 Results and Analysis
- **Approach 1**: Baseline keyword matching showed reasonable performance but lacked contextual understanding.
- **Approach 2**: BioBERT improved contextual relevance and semantic understanding but was computationally expensive.
- **Approach 3**: FAISS improved retrieval speed while maintaining high semantic accuracy.
- **Approach 4**: Hybrid model (BM25 + BioBERT) showed the best performance by balancing speed and contextual relevance.

---

## 🔍 Evaluation Metrics
- **Precision**
- **Recall**
- **Cosine Similarity Scores**

