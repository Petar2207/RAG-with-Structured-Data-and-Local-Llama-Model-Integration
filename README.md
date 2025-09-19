# 🧠 **RAG with Structured Data and Local Llama Model Integration**

This project leverages **Retrieval-Augmented Generation (RAG)** with structured data and integrates local **Llama models** for processing and classification tasks. The goal is to preserve structured data and efficiently process it for NLP applications while ensuring privacy by using local models. It is also adapted to utilize **GPU** for better performance during model inference.

## 🎯 **Project Goal**

**Primary Objective**:  
To process **structured data** in **Excel** and **JSON format**, utilizing local **Llama models** to generate document-based insights and assist with classification tasks. The system allows for effective interaction with structured data, while preserving the original structure for later use in tasks such as classification and model training.

### Key Components:
- **Structured Data Processing**: Excel data is processed and converted into structured JSON format.
- **Document JSON Preparation**: Structured data is transformed into document-based JSONs for classification.
- **Local Llama Model Integration**: The Llama model is used locally to process the data and generate insights.
- **Chat Helper Loop**: A specific loop is created for assisting with chat-based interactions, allowing for dynamic responses.
- **GPU Adaptation**: The project is adapted to use **GPU** for faster model inference when available.

---

## ✅ **Workflow Summary**

### 1. **Environment Setup & Package Installation**
- Installed essential libraries like `langchain`, `FAISS`, `pandas`, `openpyxl`, `huggingface_hub`, and `llama_cpp`.
- Set up environment-specific dependencies to enable the use of **local Llama models** for privacy and performance.
- Ensured model installation and environment configurations, especially for the local use of the **Qwen2.5 model** with **GPU support** for faster processing.

### 2. **Data Handling & Preprocessing**
- **Excel Data Processing**: Loaded structured Excel files, handled missing values, and standardized the data for conversion to JSON format.
- **Document JSON Preparation**: Structured data is converted into labeled **JSON documents** to facilitate further use in classification tasks.
- **Two Loops**:
  - One loop is dedicated to processing **Excel data** and converting it into structured JSON.
  - Another loop is designed for **chat-based interactions** to help process document-related insights using a helper function for queries.

### 3. **Model Integration & Data Preservation**
- **Llama Model**: Installed and utilized **Llama models** locally to process the structured data.
- Preserved the original **structured data** format to ensure it is reusable and stored securely.
- Used **FAISS** for vector-based document search, ensuring efficient retrieval of relevant data during classification.

### 4. **Classification & Interaction**
- Prepared structured data for future classification tasks.
- Implemented **chat helper functionality** that allows users to interact with the data, process queries, and gain insights dynamically.

---

## ⚠️ **Known Issues & To-Do**

- **Model Performance**: Check the performance of the Llama models with larger datasets to ensure efficiency.
- **Data Encoding**: Ensure that all structured data is correctly encoded in JSON format for later use in classification.
- **Error Handling**: Add additional error handling for cases when structured data cannot be processed correctly.
- **Optimization**: Investigate further optimizations for data retrieval and Llama model inference.

---

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
