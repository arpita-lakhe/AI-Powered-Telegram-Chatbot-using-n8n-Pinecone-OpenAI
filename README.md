🤖 AI-Powered Telegram Chatbot using n8n, Pinecone & OpenAI

This project is an AI-driven Telegram chatbot that uses Retrieval-Augmented Generation (RAG) to answer user queries based on documents stored in Google Drive.
The entire pipeline is automated using n8n workflows, enabling real-time document ingestion, vector storage, and intelligent responses.

🚀 Project Overview

The system automatically:

Detects new files uploaded to Google Drive

Downloads and processes documents

Splits text into chunks

Generates embeddings using OpenAI

Stores vectors in Pinecone

Responds to user queries via a Telegram bot using semantic search

This allows users to ask natural language questions and receive accurate, context-aware answers from their documents.

🧠 Architecture (RAG Pipeline)

Google Drive → n8n → OpenAI Embeddings → Pinecone Vector DB → AI Agent → Telegram Bot

🔧 Tech Stack

n8n – Workflow automation

Google Drive API – File ingestion

OpenAI API – Embeddings & Chat Model

Pinecone – Vector database

Telegram Bot API – User interaction

RAG (Retrieval-Augmented Generation) – Intelligent Q&A

⚙️ Workflows Explanation
📂 Workflow 1: Document Ingestion

Google Drive Trigger (file created)

File download

Text splitting using Recursive Character Text Splitter

OpenAI embeddings generation

Store vectors in Pinecone

💬 Workflow 2: Telegram Chatbot

Telegram Trigger (user message)

AI Agent powered by OpenAI Chat Model

Pinecone used as a retrieval tool

Semantic search over stored embeddings

Intelligent response sent back to Telegram

📸 Screenshots
<img width="656" height="440" alt="telegram3" src="https://github.com/user-attachments/assets/46bb55af-112b-43ab-8458-820ca8efc51b" />
<img width="809" height="383" alt="telegram2" src="https://github.com/user-attachments/assets/82585fb3-2642-4c9e-b53c-fc0fca39842d" />
<img width="807" height="383" alt="telegram1" src="https://github.com/user-attachments/assets/e718cbe3-ac44-4500-b336-32fec12fbd95" />





🎯 Features

Fully automated document processing

Semantic search using vector embeddings

Context-aware AI responses

Real-time Telegram chatbot

Scalable and modular workflow design

🧪 Example Use Case

User: What is Data Science?
Bot: Responds with an accurate explanation extracted from uploaded documents using vector similarity search.

📌 How to Run This Project

Set up n8n

Configure API keys:

OpenAI

Pinecone

Telegram Bot

Create Pinecone index

Import workflows into n8n

Upload documents to Google Drive

Start chatting with the Telegram bot 🎉

📚 Learning Outcomes

Hands-on experience with RAG architecture

Understanding vector databases and embeddings

Workflow automation using n8n

Building real-world AI agents

Integrating GenAI with messaging platforms

🔮 Future Enhancements

Multi-file source support

Role-based access control

Improved response ranking

UI dashboard for document management

Support for PDFs, DOCX, and web URLs

👩‍💻 Author

Arpita Lakhe
B.Sc. Computer Science
Aspiring Data Scientist | AI & GenAI Enthusiast

⭐ Acknowledgements

OpenAI

Pinecone

n8n Community
