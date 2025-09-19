# 🧠 **RAG with Structured Data and Local Llama Model Integration**

This project leverages **Retrieval-Augmented Generation (RAG)** with structured data and integrates local **Llama models** for processing and classification tasks. The goal is to preserve structured data and efficiently process it for NLP applications while ensuring privacy by using local models. It is also adapted to utilize **GPU** for better performance during model inference.

## 🎯 **Project Goal**

**Primary Objective**:  
To process **structured data** in **Excel** and **JSON format**, utilizing local **Llama models** to generate document-based insights and assist with classification tasks. The system allows for effective interaction with structured data, while preserving the original structure for later use in tasks such as classification and model training.

### Key Components:
- **Excel Data Processing**: The data from the Excel file is converted into **row_dict** objects. Each row is turned into a **combined string** with fields like `x`, `y`, `z`, which is then sent to the model for processing.
- **Document Preparation**: The structured data is converted into **Langchain documents** for classification and further processing.
- **Local Llama Model Integration**: The Llama model is used locally to process the data and generate insights.
- **Chat Helper Loop**: I wrote code (commented as `#`) that edits the structured JSON file and prepares it for dynamic interactions. This is followed by a loop that processes chat queries, allowing the user to interact with the structured data dynamically. The loop assists in analyzing the data and generating responses based on the user’s input.

- **GPU Adaptation**: The project is adapted to use **GPU** for faster model inference when available.

---

## ✅ **Workflow Summary**

### 1. **Environment Setup & Package Installation**
- Installed essential libraries like `langchain`, `FAISS`, `pandas`, `openpyxl`, `huggingface_hub`, and `llama_cpp`.
- Set up environment-specific dependencies to enable the use of **local Llama models** for privacy and performance.
- Ensured model installation and environment configurations, especially for the local use of the **Qwen2.5 model** with **GPU support** for faster processing.

### 2. **Model Integration & Data Preservation**
- **Llama Model**: Installed and utilized **Llama models** locally to process the structured data.
### 3. **Data Handling & Preprocessing**
- Used **FAISS** for vector-based document search, ensuring efficient retrieval of relevant data during classification.

### 4. **Classification**
- Prepared structured data for future classification tasks.

## 🛠️ **Tech Stack**

- **Languages**: Python
- **Libraries**: `langchain`, `FAISS`, `pandas`, `openpyxl`, `huggingface_hub`, `llama_cpp`, `json`, `tqdm`, and more.

---

## 📜 **License**

This project is licensed under the **MIT License** — free to use and modify.

---

## 👤 **Author**

Petar Rajic

To install required libraries:

```bash
pip install langchain faiss-cpu pandas openpyxl huggingface_hub llama-cpp
