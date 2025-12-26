# LangChain RAG Chatbot (FAISS + Gemini)

A simple Retrieval-Augmented Generation (RAG) chatbot built using **LangChain**, **FAISS**, and **Google Gemini**.  
It lets you chat with your own documents by retrieving the most relevant content and generating responses using Gemini models.

## What it does
- Loads and processes HTML documents  
- Creates embeddings using Gemini  
- Stores them in a FAISS vector index  
- Retrieves relevant chunks for each query  
- Generates grounded answers using LangChain + Gemini  
- Supports multi-query search, question breakdown, and basic chat memory

## Quick Start
1. Clone the repo and install dependencies:
```bash
pip install langchain_community
pip install faiss-cpu
pip install langchain_google_genai
pip install unstructured
pip install python-dotenv
```   
2. Add your Gemini API key in a .env file:
```bash
GEMINI_API_KEY=your_api_key_here
```
3. Place your HTML files in the coffee_pages/ folder.

4. Run the notebook (P1.ipynb) in Colab or locally to start the chatbot.

## Example queries
What is Ashwagandha coffee?
Compare Ashwagandha and mushroom coffee.
Summarize the main ingredients mentioned.

## Project structure 
```bash
langchain-rag-faiss-chatbot/
├── coffee_pages/     # your HTML files
├── P1.ipynb          # main RAG notebook
├── faiss_index/      # generated vector store
└── README.md
```
## About 
Built as a hands-on demo to explore document-based chat using LangChain and FAISS with Gemini models.
