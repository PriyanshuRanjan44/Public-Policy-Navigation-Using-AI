# 📂 Virtual File Space

An interactive **Streamlit application** that allows you to upload, process, and query files using **chunking + embeddings + Ollama-powered conversational AI**.  

With this app, you can:
- Upload multiple files (PDF, DOCX, CSV, TXT, JSON, images, etc.)
- Automatically **chunk** and embed documents for retrieval
- Save chunked text as **JSON**
- Ask natural language questions and get contextual answers
- Manage sessions with a simple and clean UI

---

## 🚀 Features

- **Multi-file Upload**: Supports `pdf`, `docx`, `csv`, `txt`, `json`, and more  
- **Smart Chunking**: Split documents into chunks of configurable size  
- **Embeddings + Retrieval**: Uses [SentenceTransformers](https://www.sbert.net/) and [FAISS](https://faiss.ai/) for semantic search  
- **Conversational Q&A**: Query your documents using an **Ollama-powered LLM**  
- **Session Management**: Clear history, save uploads, and track session inventory  
- **Download Chunks**: Export processed chunks as a JSON file  

---

## 🛠️ Installation

# 1. Clone the repository
git clone https://github.com/your-username/virtual-file-space.git
cd virtual-file-space

# 2. Create and activate a virtual environment
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run the app
streamlit run app.py

---

## 📦 Dependencies

```text

├── Streamlit              # Web Interface  
├── SentenceTransformers   # Embedding model  
├── faiss-cpu              # Vector index for retrieval  
├── pandas                 # Data handling  
├── numpy                  # Numerical operations  
└── ollama                 # LLM query engine

### Additional project modules:

ocr.py                # For PDF/DOCX processing
ollama_client.py      # For interacting with Ollama
```

---

## 📖 Usage

1. streamlit run app.py  # Start the app

2. **Upload one or more documents**  
3. The app will:  
   - Detect type (PDF/DOCX/etc.)  
   - Chunk and embed content  
   - Save chunks to `.json`  
   - Display session inventory  
4. **Ask questions** in the chat input and get context-aware answers  
5. **Optionally download** the processed chunks   

---

## 📂 Project Structure

```text
├── app.py              # Main Streamlit app (Virtual File Space)
├── ocr.py              # Document parsing (DOCX/PDF to text chunks)
├── ollama_client.py    # Interface with Ollama models
├── requirements.txt    # Python dependencies
├── uploads             # Uploaded files (session-specific)
└── README.md           # Documentation
```

---

## 📜 License

MIT License

Copyright (c) 2025 Priyanshu Ranjan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

---
