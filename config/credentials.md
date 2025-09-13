# Credentials Setup (Do Not Commit Secrets)

⚠️ Never put real tokens or API keys in GitHub. Use n8n's credential manager.

### Required Credentials

- Google Gemini API → Add key in n8n under "GooglePalmApi".
- Postgres → Add DB connection string in n8n.
- WhatsApp Business API → Meta App ID + Permanent Access Token.
- Qdrant → Localhost or hosted endpoint connection.
- Ollama → Local LLM instance (if used).

### How to Add

1. Open n8n UI → Credentials.
2. Create each credential with the name expected in the workflow.
3. Test each connection before activating workflow.
