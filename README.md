# **VivoMeetings Chatwoot Fork**

### *Enterprise-Grade Customer Support Platform with AI Automation & Human Handoff*

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
![Status](https://img.shields.io/badge/Status-Active-blue)
![Platform](https://img.shields.io/badge/Platform-Self--Hosted-important)
![AI Powered](https://img.shields.io/badge/AI-Powered-brightgreen)

## 📘 **Overview**

The VivoMeetings Chatwoot Fork is an **enterprise-customized**, **open-source** version of Chatwoot engineered to support large-scale customer communication workflows within the VivoMeetings ecosystem.

This distribution enhances Chatwoot with:

* **AI-assisted automated responses** powered by OpenAI
* **Real-time human agent takeover** for escalations
* **Multi-channel communication** for business environments
* **Branding and workflow enhancements** tailored for SaaS companies
* **Full self-hosting** for organizations requiring privacy, compliance, and data sovereignty

This fork maintains compatibility with upstream Chatwoot while offering additional enterprise features.

## 🚀 **Key Enterprise Features**

### 🤖 **AI Automation Layer**

* OpenAI-powered response engine
* Low-confidence detection and escalation
* Knowledge-base inference for instant answers
* Configurable prompt architecture for domain-specific support

### 🧑‍💼 **Human Agent Escalation**

* Seamless transition from bot to human
* SLA-driven routing and assignment
* Private internal notes for agent collaboration
* Supervisor visibility for escalated conversations

### 📡 **Omnichannel Support**

* Web chat widget
* Email channels
* API-driven integrations
* Future expansion for WhatsApp, Telegram, and SMS

### 🔐 **Security & Compliance**

* Fully self-hosted
* MIT-licensed open-source
* GDPR-aligned workflows
* Suitable for enterprise internal deployments

### 🏢 **SaaS-Ready Enhancements**

* Custom theming and branding
* Robust API middleware for scalable automation

---

## 🧱 **Architecture Overview**

                  ┌───────────────────────────┐
                  │   VivoMeetings Platform    │
                  └──────────────▲────────────┘
                                 │
                                 │ API / Webhooks
                                 │
                    ┌────────────┴────────────┐
                    │   Chatwoot (Core Fork)   │
                    │  Routing, UI, Inboxes    │
                    └───────▲─────────┬────────┘
                            │         │
       Human Interaction    │         │    AI Automation
                            │         │
                 ┌──────────┘         └───────────┐
                 │                                 │
  ┌──────────────┴──────────────┐   ┌──────────────┴───────────────┐
  │    Agent Dashboard (UI)      │   │      OpenAI Bot Service       │
  │ Real-time responses & notes  │   │ AI Reply, Confidence Scoring  │
  └──────────────────────────────┘   └───────────────────────────────┘


## ⚙️ **Installation & Deployment**

This fork follows the official Chatwoot self-hosting documentation:

### **1. Clone the repository**

```bash
git clone https://github.com/vivomeetings/chatwoot.git
cd chatwoot
```

### **2. Follow upstream setup guide**

Documentation:
[https://www.chatwoot.com/docs/self-hosted](https://www.chatwoot.com/docs/self-hosted)

Supports:

* Docker / Docker Compose
* Kubernetes
* Bare-metal installs

### **3. Configure OpenAI Bot Service**

Connect the bot using Webhook-based Agent Bot:

* Bot middleware URL (your AI service)
* Chatwoot API token
* OpenAI API key

## 🔧 **Environment Variables (AI Integration)**

```env
OPENAI_API_KEY=your_openai_key
CHATWOOT_API_TOKEN=your_chatwoot_token
CHATWOOT_BASE_URL=https://support.yourdomain.com
BOT_WEBHOOK_URL=https://your-bot-service.com/chatwoot
```

## 📦 **Recommended Deployment Stack**

| Component            | Purpose                  |
| -------------------- | ------------------------ |
| **Chatwoot**         | Core messaging engine    |
| **PostgreSQL**       | Persistent storage       |
| **Redis**            | Job processing + caching |
| **AI Bot Service**   | OpenAI integration layer |
| **NGINX / Ingress**  | Reverse proxy + SSL      |
| **Docker + Compose** | Self-hosting simplicity  |


## 🛡️ **Enterprise Use Cases**

* Customer support automation
* SaaS onboarding assistants
* Technical support triage
* Internal IT helpdesk

## 🤝 **Contributing**

We welcome enterprise collaborators, integrators, and open-source contributors.

Please submit:

* Pull requests
* Feature suggestions
* Integration modules

## 📄 **License**

This project is released under the **MIT License**, allowing commercial and enterprise usage with attribution.

See the full [LICENSE](LICENSE) file for details.


## 🌍 **Contact & Links**

* **Chatwoot Upstream:** [https://github.com/chatwoot/chatwoot](https://github.com/chatwoot/chatwoot)
* **Issues / Requests:** GitHub Issues tab


## ⭐ **Maintained by VivoMeetings Engineering**

Building secure, scalable communication tools for modern SaaS platforms.


