# 🚀 WorkShop_Project_Metavers

This repository was created as part of my final-year internship (PFA) at **Metacerse**.  
The goal of this workshop is to explore the capabilities of **Large Language Models (LLMs)**, including fine-tuning and enhancing their responses using **RAG (Retrieval-Augmented Generation)** techniques.

---

## 🗂️ Repository Structure

### 📁 DataSets
This folder contains datasets used throughout the project:

- **DeepSeek Conversations (`.json`)**:  
  Generated conversations using the DeepSeek API, stored in JSON format. This dataset is dynamically updated during execution of the notebooks.

- **GooAQ Dataset (`.txt`)**:  
  A dataset from Hugging Face containing real-world user queries extracted from Google search. It is stored in plain text format and used for fine-tuning.

---

### 📁 PdfsDocs
Contains PDF documents used in **Lab 3**.  
These documents are embedded and stored in **ChromaDB** to support **RAG pipelines**, improving response quality from the Mistral-7B model through context retrieval.

---

### 📓 Notebooks

#### `LAB_1_Create_data_set.ipynb`
- Setups a basic pipeline with the **DeepSeek API** to execute queries.
- Parses and stores responses in JSON format.
- Implements custom functions to organize and save conversations.

#### `LAB_2_fine-tune-gpt-2-lmm.ipynb`
- Focuses on fine-tuning the **GPT-2 model** using Hugging Face's Transformers.
- Two fine-tuning approaches:
  1. Using the generated **DeepSeek JSON** dataset.
  2. Using the **GooAQ text dataset**.
- Includes **LangChain-based pipeline** for:
  - Saving question-answer pairs to **ChromaDB**
  - Enhancing model's retrieval for repeated questions.

#### `LAB-3-LLm-and-pdfs-preprocessing.ipynb`
- Utilizes the **Mistral 7B model** from **Mistral AI**.
- Two RAG-based approaches:
  1. Basic RAG with custom embedding + retrieval logic.
  2. Predefined RAG pipeline from `langchain.chains`.
- Final pipeline answers user questions by retrieving content embedded from PDFs stored in ChromaDB.

---

## 🧠 Key Concepts
- **RAG (Retrieval-Augmented Generation)**
- **LLMs (GPT-2, Mistral-7B, DeepSeek)**
- **Fine-Tuning using Hugging Face**
- **LangChain & ChromaDB Integration**
- **Semantic Search & Embedding Techniques**

---

## 🛠️ Tech Stack
- Python
- Hugging Face Transformers
- LangChain
- ChromaDB
- Mistral AI (7B)
- DeepSeek API
- Jupyter Notebooks

---

## 📌 Acknowledgements
- [Metacerse](https://metacerse.com) for the internship opportunity  
- Hugging Face, LangChain, and Mistral AI for open-source tools

---

## 📫 Contact
For any inquiries or questions, feel free to reach out:

**Mohamed Amhal**  
💼 Data Science & AI Engineer  
📧 [Insert your email or LinkedIn]

