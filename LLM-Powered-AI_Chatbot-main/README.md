Shiva – AI-Powered Document Assistant

An AI-powered conversational application that uses Retrieval-Augmented Generation (RAG) to answer questions based on uploaded documents.

Shiva combines a React frontend, Node.js backend, MongoDB database and Groq LLM API to provide document-based question answering.



- Upload PDF, DOCX and TXT documents.
- Extract and process document text.
- Split documents into smaller text chunks.
- Generate embeddings locally.
- Retrieve relevant document passages using cosine similarity.
- Generate contextual answers using Groq LLaMA.
- Display source document references.
- Stream AI responses.
- Maintain conversational history.
- Dark and light themes.
- Export chat history.

Technology Stack

Component| Technology
Frontend| React, CSS
Backend| Node.js, Express.js
Database| MongoDB Atlas
AI Model| Groq LLaMA
Embeddings| Transformers.js
PDF Processing| pdf-parse
DOCX Processing| mammoth
Development| Nodemon

How RAG Works

1. Document ingestion: Users upload documents.
2. Text extraction: Text is extracted from supported files.
3. Chunking: Extracted content is divided into smaller overlapping sections.
4. Embedding generation: Text chunks are converted into numerical vectors.
5. Retrieval: Relevant chunks are selected using cosine similarity.
6. Augmentation: Retrieved content is added to the LLM prompt.
7. Generation: The LLM generates an answer using the retrieved context.

Installation

Prerequisites

- Node.js 18 or later
- MongoDB connection string
- Groq API key
- Git

Backend Setup

cd backend
npm install

Create a ".env" file inside the backend folder:

GROQ_API_KEY=your_groq_api_key
MONGO_URI=your_mongodb_connection_string
PORT=5000

Start the backend:

npm run dev

Frontend Setup

Open another terminal:

cd frontend
npm install
npm start

Open:

"http://localhost:3000"

Environment Variables

Variable| Description
GROQ_API_KEY| Groq API credentials
MONGO_URI| MongoDB connection
PORT| Backend server port

Future Improvements

- User authentication and authorization.
- Private document storage for individual users.
- Improved semantic retrieval.
- MongoDB Atlas Vector Search.
- Document management dashboard.
- Automated testing and API documentation.

Contributions

Document your own work here:

- Features independently implemented:
- Bugs fixed:
- UI improvements:
- Backend enhancements:
- Testing performed:

