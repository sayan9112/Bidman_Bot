# Local AI Chatbot (Complete Version)

## Overview
This project provides a local AI chatbot that analyzes large codebases using LangChain for context-aware answers and Angular Material for UI.

### Features
- Upload multiple files or folders
- Context-aware answers using LangChain + FAISS
- Angular Material UI
- Runs completely offline

### Setup
1. Install Python 3.10+
2. Install Node.js and Angular CLI
3. Install Ollama and pull Code Llama model:
   ```bash
   ollama pull codellama
   ```
4. Backend:
   ```bash
   cd backend
   pip install -r requirements.txt
   uvicorn main:app --reload
   ```
5. Frontend:
   ```bash
   cd frontend
   npm install
   ng serve
   ```

### Notes
- Replace `sk-REPLACE_WITH_KEY` in main.py with your OpenAI API key for embeddings.



# After creating Angular app:
npm install @angular/material @angular/cdk @angular/animations
ng add @angular/material
