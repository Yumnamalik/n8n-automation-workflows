# 💬 Lead Qualifier - Classify Incoming Leads via WhatsApp

An automated n8n workflow that captures incoming leads from Typeform, uses Google Gemini AI to analyze and classify lead sentiment (Hot, Neutral, Cold), routes and logs the lead data, and sends an automated WhatsApp response.

![Workflow Canvas](./workflow.png)

## 🌟 Key Features
- **Trigger**: Receives new lead submissions via Typeform.
- **AI Sentiment Analysis**: Uses Google Gemini Chat Model and Structured Output Parser to classify leads into Hot, Neutral, or Cold.
- **Dynamic Routing**: Routes leads based on sentiment score/category to update lead databases accordingly.
- **Automated Messaging**: Sends custom WhatsApp template messages automatically via WhatsApp Business API.

## 🛠️ Prerequisites
- **n8n Instance** (Self-hosted or n8n Cloud)
- **Typeform Account** & API connection
- **Google AI Studio API Key** (for Gemini)
- **WhatsApp Business API Account**

## 🚀 Quick Setup
1. Download `workflow.json` from this directory.
2. In n8n, click **Workflows** > **Import from File** and select `workflow.json`.
3. Re-link your credentials for Typeform, Google Gemini, and WhatsApp.
4. Activate the workflow toggle.
