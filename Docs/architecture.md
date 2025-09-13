# WhatsApp AI Agent – Architecture

This document explains the structure of the n8n workflow.

### Nodes

- WhatsApp Trigger – Captures incoming messages from WhatsApp Business Cloud API.
- AI Agent – Orchestrates decision-making and routes messages.
- Google Gemini Chat Model – Provides natural language responses.
- Postgres Chat Memory – Stores past conversations for context.
- Google Drive File Download – Retrieves company FAQs or reference docs.
- Qdrant Vector Store – Handles embeddings for semantic search.
- Send WhatsApp Message – Sends AI response back to the user.

### Flow

Incoming WhatsApp → Pre-processing → Query knowledge base (Gemini + Qdrant) → Memory check (Postgres) → Respond through WhatsApp.
