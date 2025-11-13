


# **Bidman Bot – Local AI-Powered Code Analysis Chatbot**

## **Introduction**
Bidman Bot is an **offline AI-powered chatbot** designed to analyze large codebases and provide actionable coding solutions. Unlike cloud-based systems, this chatbot runs entirely on **local infrastructure**, ensuring **data privacy**, **security**, and **offline availability**.

It supports large folders (700 MB – 1 GB) containing multiple file types such as `.cs`, `.html`, `.ts`, `.json`, and more.  
The chatbot assists developers by:
- Understanding complex code structures.
- Suggesting debugging tips and enhancements.
- Supporting **.NET**, **Angular**, and other technologies.

The system will be deployed internally, allowing multiple team members to download and run it from a shared GitHub repository.

---

## **Core Objectives**
- Enable multi-file and folder uploads for large projects.
- Provide context-aware code analysis using local AI models.
- Operate completely offline without cloud dependencies.
- Ensure secure access within the office network.

---

## **Functional Requirements**
### 1. File and Folder Upload
- Drag-and-drop interface for uploading entire folders.
- Support for mixed file types and large sizes.

### 2. Code Analysis
- Understand **.NET** and **Angular** code.
- Provide suggestions for optimization and debugging.

### 3. Context Management
- Use chunking and embeddings for large codebases.
- Maintain session context for multi-file queries.

### 4. Local Execution
- No external API calls.
- Runs on office servers or developer machines.

---

## **Non-Functional Requirements**
- **Performance:** Efficient handling of 1 GB code folders.
- **Security:** Local authentication (JWT or LDAP).
- **Scalability:** Allow multiple users to run the system locally.

---

## **System Requirements**
### Hardware
- **CPU:** 8 cores minimum.
- **RAM:** 16 GB (32 GB recommended).
- **Storage:** 50–100 GB free space.
- **GPU:** NVIDIA GPU with 8 GB+ VRAM (optional for faster inference).

### Software
- **OS:** Windows/Linux/macOS.
- **Python:** 3.10+
- **Node.js & Angular CLI**
- **FastAPI**
- **LangChain / LlamaIndex**
- **Vector DB:** FAISS or Chroma.
- **Local LLM Runner:** Ollama or GPT4All.
- **Dependencies:** PyTorch, Transformers.

### Model
- **Code Llama** or **StarCoder** (~7–13 GB).

---

## **Installation Guide**
### **Step 1: System Requirements**
Ensure your machine meets the hardware and software requirements listed above.

---

### **Step 2: Install Prerequisites**
#### 2.1 Install Python
Download and install Python 3.10+ from https://www.python.org/downloads/.  
Verify installation:
```bash
python --version
