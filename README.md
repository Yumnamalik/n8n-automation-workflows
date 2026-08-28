# ⚡ n8n Automation Workflows

A collection of production-ready n8n automation workflows covering AI agents, lead generation, document processing, and web scraping.

---

## 📂 Included Workflows

| Workflow | Category | Key Tech / APIs | Description |
| :--- | :--- | :--- | :--- |
| 🚀 **[Lead Generation with Snov.io](./lead-generation-snov)** | Lead Gen & Outreach | Snov.io, n8n | Automates lead enrichment, email extraction, and prospect list building. |
| 🤖 **[RAG Chatbot for Company Documents](./rag-chatbot-drive-gemini)** | AI & Knowledge Base | Google Drive, Google Gemini, Pinecone | Ingests company docs from Google Drive, stores embeddings in Pinecone, and powers an AI chat assistant. |

---

## 🛠️ Requirements & Setup

1. **n8n Instance**: Self-hosted (Docker/n8n Cloud) or local instance.
2. **Importing Workflows**:
   - Navigate to any workflow directory above.
   - Download the `workflow.json` file.
   - In your n8n canvas, click **Workflows** > **Import from File**.
3. **Credentials**: Each workflow directory contains specific credential requirements in its respective `README.md`.
