# HelpMate AI

> **AI-powered chatbot to assist with insurance policy documents.**  

---

## 📚 About the Project
RAG Insurance Assistant (HelpMate AI) is an innovative solution crafted to simplify the process of understanding and extracting information from complex insurance documents.

Traditional methods of sifting through lengthy policy documents, claim guidelines, and legal jargon are often time-consuming and frustrating for users.
HelpMate AI eliminates these challenges by leveraging Retrieval-Augmented Generation (RAG) — a cutting-edge approach that combines semantic information retrieval with natural language generation from advanced AI models.

With HelpMate AI, users can ask natural, everyday questions and receive clear, citation-backed answers directly sourced from their insurance documents.

🎯 Example Use Cases
"What is covered under my health insurance policy?"

"How can I file a claim for vehicle insurance?"

"What exclusions should I be aware of in my travel insurance?"

"What documents are required to file a hospitalization claim?"


---

## Features

- Extracts structured content (text, headings, tables) from PDF documents.
- Divides text into manageable chunks with metadata like page numbers and sections.
- Generates semantic embeddings using OpenAI’s `text-embedding-ada-002`.
- Stores and retrieves data efficiently with **ChromaDB**.
- Reranks search results with a **cross-encoder model** for better accuracy.
- Generates natural, informative responses using **GPT-4o-mini**, including document citations.
- Implements caching for faster response times on repeated queries.
- Provides an interactive chatbot experience.

---

## 🛠️ Tech Stack

| Purpose                  | Technology                           |
|---------------------------|--------------------------------------|
| PDF Text Extraction       | `pdfplumber`                        |
| Embedding Model           | OpenAI `text-embedding-ada-002`      |
| Vector Database           | `ChromaDB`                          |
| Reranking                 | Cross-Encoder (e.g., HuggingFace)    |
| Response Generation       | OpenAI `gpt-4o-mini`                 |
| Programming Language      | Python                              |
| Frontend (Optional)       | Streamlit / React (to be implemented) |
| Backend (Optional)        | FastAPI / Flask (to be implemented) |

---

## ⚙️ System Architecture

```
PDF Document ➔ Text Extraction ➔ Chunking + Metadata ➔ Embedding + Indexing ➔
User Query ➔ Query Embedding ➔ Semantic Search + Reranking ➔
Response Generation ➔ Caching ➔ User Interface
```

---

## 🚀 Getting Started

> *Note: Version 1 is the initial submission. Future enhancements will be rolled out in V2.*

### Prerequisites
- Python 3.9+
- OpenAI API key
- ChromaDB installed locally or cloud-based
- Required Python libraries (see `requirements.txt`)

### Installation

```bash
git clone https://github.com/akaashmk/helpmate-ai.git
cd helpmate-ai
pip install -r requirements.txt
```

### Configuration
- Add your OpenAI API key in a `.env` file:

```plaintext
OPENAI_API_KEY=your_openai_api_key
```



## 📢 Acknowledgements

- UpGrad and IIIT Bangalore – for the AI and ML PG Program.
- OpenAI – for powerful embedding and GPT models.
- ChromaDB – for seamless vector search capabilities.

---

## 📬 Contact

For any queries or feedback, feel free to reach out:

- Email: akaashmk@gmail.com
- GitHub: https://github.com/akaashmk/
- LinkedIn: www.linkedin.com/in/akaashkarthikeyan

---
