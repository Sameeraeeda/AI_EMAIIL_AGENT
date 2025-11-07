# AI_EMAIIL_AGENT
🧠 AI Email Agent – Daily Email Digest Automation
🚀 Overview

This project automates email management using AI + automation + APIs.
Every morning at 9 AM, an AI Email Agent fetches your Gmail inbox, summarizes key emails, categorizes them, and delivers a clean daily digest directly to Telegram and WhatsApp — so you never need to check your inbox manually.
<img width="1100" height="550" alt="image" src="https://github.com/user-attachments/assets/3babec75-7784-4300-9b33-d8d3ce97bccf" />

⚙️ Workflow Summary
Step	Component	Description
1️⃣	n8n Schedule Trigger	Starts workflow daily at 9:00 AM
2️⃣	Gmail API	Fetches new emails from the last 24 hours
3️⃣	Data Extractor	Cleans and structures email data (JSON format)
4️⃣	Google Gemini AI	Summarizes, categorizes (Work, Finance, Personal, Promotions), and prioritizes
5️⃣	Formatter	Builds clean, emoji-friendly digest text
6️⃣	Telegram Bot API	Sends digest message to Telegram
7️⃣	Twilio WhatsApp API	Sends same digest message to WhatsApp
🧩 Tech Stack
Tool / API	Purpose
n8n	Workflow automation and scheduling
Gmail API	Fetches inbox emails
Google Gemini 2.0 Flash	AI summarization & classification
Telegram Bot API	Message delivery to Telegram
Twilio WhatsApp API	Message delivery to WhatsApp

🧰 Setup Instructions
1️⃣ Prerequisites

n8n installed locally or on server

Google Cloud Project with Gmail API enabled

Google Gemini API key

Telegram Bot Token (@BotFather)

Twilio Account with WhatsApp sandbox

2️⃣ Import Workflow

Open n8n Dashboard → Import > Paste JSON

Use the provided ai-email-agent-workflow.json

Replace:

"YOUR_BOT_TOKEN" → your Telegram bot token  
"YOUR_TWILIO_SID" → your Twilio Account SID  


Add credentials for:

Gmail API OAuth

Gemini API Key

Twilio WhatsApp API

3️⃣ Activate Schedule

Enable workflow

Runs automatically every day at 9:00 AM

📨 Output Example
📧 Daily Email Digest

🔔 Important
• Debit Alert ₹2000 — ₹2000 debited from HDFC. [High]
  → Action: Verify transaction in banking app.

💼 Work
• Meeting Invite — Reschedule 1:1 requested. [Medium]
  → Action: Propose new time for tomorrow.

🌟 Why It’s Useful

✅ Saves time — no need to open Gmail
✅ Keeps inbox stress-free
✅ Uses AI for intelligent filtering
✅ Works across platforms (Telegram, WhatsApp)

🔮 Future Enhancements

 Slack integration

 Notion / Google Calendar sync

 PDF digest export

 Voice summary using TTS
