# 🧠 AI Job Hunting Assistant (n8n + OpenAI + Google sheets + Gmail)

A fully automated job hunting assistant powered by **n8n**, integrated with **OpenAI**, and **Google Workspace**. 
It fetches new job listings, evaluates them against personal profile with scores, lets you approve the preferable jobs via Gmail, 
the approved ones will continue to the automation to generate custom cover letters.


---

## 📌 Features

* ⏰ **Runs twice daily** to fetch LinkedIn, jobs via RSS (scalable to more websites Glassdoor, Duunitori)
* 🤖 **Parses job content** from HTML via HTTP Request + OpenAI
* 📊 **Matches jobs with your profile** using OpenAI GPT
* ✅ **Approval via Gmail** (one-click approve/decline)
* ✍️ **Generates personalized cover letters**
* 📄 **Writes to Google Sheets**

---

## 🧱 Tech Stack

* `n8n` – Workflow Automation
* `OpenAI GPT-4` – Matching & Cover Letter Generation
* `Google Sheets, Docs, Gmail` – Output & Communication
* `Docker` – Deployment

---

## 🚀 Quick Start (Use via n8n Cloud)

1. 🆓 Go to [n8n.cloud](https://n8n.cloud) and create a free account
2. 🔐 Set up your API keys and credentials via the UI:
   - OpenAI API Key
   - Telegram Bot Token
   - Google OAuth (Sheets, Docs, Gmail)
3. 📤 Import the workflow:
   - Go to “Workflows” → “Import” → Upload [`main-jobhunt-workflow.json`](workflows/main-jobhunt-workflow.json)
4. 🛠️ Modify parameters like schedule time, keywords, Telegram chat_id
5. ✅ Activate the workflow

> No need to install anything locally. Everything runs on n8n Cloud.

