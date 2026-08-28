# RAG Chatbot for Company Documents (Google Drive + Gemini + Pinecone)

An automated n8n workflow that watches a Google Drive folder for document uploads/updates, embeds and stores the text in a Pinecone vector index, and provides an interactive AI Chatbot using Google Gemini to answer questions based on your internal documentation.

## Features
- **Automatic Document Ingestion**: Triggers when files are created or updated in a specified Google Drive folder.
- **Vector Indexing**: Chunks text using Recursive Character Text Splitter and stores embeddings in Pinecone using Google Gemini Embeddings.
- **AI Agent Chatbot**: Uses `gemini-3.5-flash` with buffer memory to answer queries via an n8n chat interface.

## Prerequisites
- **n8n Instance** (Self-hosted or Cloud)
- **Google Cloud Project** with Vertex AI / Google AI Studio API key
- **Pinecone Account** with an index named `company-files`
- **Google Drive** folder created for document storage

## Setup Instructions

1. **Import Workflow**:
   - In n8n, click **Workflows** > **Import from File** and select `workflow.json`.

2. **Configure Credentials**:
   - **Google Drive OAuth2 API**: Link your Google Drive account.
   - **Google Gemini (PaLM) API**: Enter your Google AI Studio API key.
   - **Pinecone API**: Enter your Pinecone API key.

3. **Node Configuration**:
   - Update both **Google Drive Trigger** nodes to select your target folder.
   - Ensure the **Pinecone Vector Store** nodes point to your `company-files` index.

4. **Activation**:
   - Save and toggle the workflow to **Active**.
