# Description

This project showcases a hybrid Generative AI Chatbot capable of understanding and answering user queries based on PDF documents using both OpenAI's GPT models and Google's Gemini models.


# Key Objectives

LLM Orchestration: Integrate OpenAI and Gemini in a single notebook to support dynamic backends.

Document Intelligence: Extract context from PDF files using PyMuPDF and PyPDF2.

Conversational Flow: Enable chat-based question answering about uploaded documents.

Evaluation Ready: Makes it easy to compare and analyze answers from both LLMs side by side.


# Tools & Technologies


| Component            | Description                                     |
| -------------------- | ----------------------------------------------- |
| **OpenAI API**       | For GPT-4.1 based conversational output |
| **Gemini API**       | Google's GenAI model for reasoning and Q\&A     |
| **PyMuPDF / PyPDF2** | For accurate text extraction from PDFs          |
| **Jupyter Notebook** | Interactive and modular execution               |
| **Python 3.x**       | Core scripting language for integration         |

# How It Works

## 1) PDF Upload
User uploads one or more PDFs. The notebook uses fitz and/or PyPDF2 to extract clean text, page by page.

## 2) Prompt Construction
The extracted document content is chunked intelligently and prepended to user questions as context.

## 3) Dual-Model Inference
Based on user preference:

✅ Use OpenAI's GPT (via openai.ChatCompletion)

✅ Or Google Gemini (via google.generativeai)

## 4) Response Comparison (Optional)
Evaluate and compare answers across OpenAI vs Gemini to assess:

Accuracy

Factual correctness

Completeness

Style of response.

#  Real-World Use Cases
🔍 Legal & Compliance: Extract and explain clauses

📚 Education: Tutor bot for academic papers

🏥 Healthcare: Summarize and interact with medical reports

🛠️ Technical Support: Chatbot for user manuals.

 # Next Steps (Optional Enhancements)
1. Add embedding-based retrieval (e.g., FAISS + vector store)

2. Create a Streamlit UI for non-technical users

3. Enable multi-document ingestion

4. Add a benchmark mode to track response quality from both LLMs





