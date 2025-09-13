---

# 🤖 WhatsApp AI Agent  

![Status](https://img.shields.io/badge/Status-Active-brightgreen)  
![WhatsApp](https://img.shields.io/badge/API-WhatsApp%20Cloud-blue?logo=whatsapp)  
![n8n](https://img.shields.io/badge/Workflow-n8n-orange?logo=n8n)  
![AI](https://img.shields.io/badge/Powered%20by-AI-red?logo=openai)  

This repository contains a WhatsApp AI Agent that connects with the WhatsApp Cloud API and uses n8n workflows to process and reply to client messages automatically.  
It answers FAQs, handles client interactions, and provides instant support 💬.  

---

## 📋 Features

- ✅ Automated WhatsApp Replies
- ✅ FAQ Handling via Knowledge Base
- ✅ Seamless Integration with n8n
- ✅ AI-powered Smart Responses 🚀

---

## 📊 Workflow Diagram

Below is the workflow of how the WhatsApp AI Agent operates:

![WhatsApp AI Agent Workflow](assets/whatsapp%20AI%20Agent.png)

---

## 🚀 Step-by-Step Setup

### 1. Clone the Repository

`bash
git clone https://github.com/Ezrawambugu/Whatsapp-business-AI-Agent.git
cd whatsapp-ai-agent

2. Install Dependencies

npm install

3. Configure Environment Variables

Create a .env file in the project root and add:

WHATSAPP_API_KEY=your_whatsapp_api_key  
N8N_WEBHOOK_URL=your_n8n_webhook_url

4. Run the Bot

npm start

---

⚡ How It Works

The WhatsApp AI Agent follows this workflow:

1. 📲 User sends a message on WhatsApp.

2. ☁️ The message passes through the WhatsApp Cloud API.

3. 🔄 An n8n workflow is triggered and forwards the message.

4. 🧠 The AI Agent processes the query.

5. 📚 If needed, it searches the Knowledge Base (FAQs) for resources.

6. 📝 A text classifier checks if the agent has sufficient info to reply:

✅ If yes → The query is forwarded to the AI Agent for an instant reply.

❌ If not → The query is routed to the admin via WhatsApp Cloud. The admin responds, and the reply is routed back to the client.

7. 📧 Finally, the last AI Agent can draft and send an email with the provided information.

---

🙌 Contributing

Contributions make the community stronger 💡.

Fork the repository

Create your feature branch (git checkout -b feature/your-feature)

Commit your changes (git commit -m 'Add some feature')

Push to the branch (git push origin feature/your-feature)

Open a pull request

For major changes, please open an issue first to discuss what you’d like to change.

---

📜 License

This project is licensed under the MIT License.
You are free to use, modify, and distribute this software, provided that proper credit is given.

---
