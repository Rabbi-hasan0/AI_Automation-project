# 🤖 AI-Powered Smart Booking & Customer Support Agent

An advanced automation workflow built with **n8n** and powered by **Google Gemini AI**. This project functions as an intelligent Customer Support Agent for "SmartFlow Automations," capable of handling inquiries, managing leads, and scheduling meetings automatically.

---

## 📺 Project Overview
This system acts as a bridge between customers and business services. It doesn't just reply to messages; it understands intent, fetches service data, and takes action (like booking a calendar event) based on the conversation.

### Key Features
* **Intelligent AI Agent:** Powered by `Gemini 1.5` to provide polite, professional, and context-aware responses in Bengali/English.
* **Automated Booking:** High-priority logic to collect user details (Name, Email, Date) and sync them with **Google Calendar**.
* **Live Data Fetching:** The AI reads service descriptions and pricing logic directly from **Google Sheets**.
* **Lead Management:** Automatically saves every potential customer's information into a database (Google Sheets) for future follow-ups.
* **Memory Retention:** Includes a memory buffer so the AI remembers what the user said earlier in the chat.

---

## 🛠️ Tech Stack
| Component | Technology |
| :--- | :--- |
| **Automation Engine** | n8n |
| **AI Brain** | Google Gemini (LLM) |
| **Database** | Google Sheets |
| **Scheduling** | Google Calendar API |
| **Trigger** | Webhooks (REST API) |

---

## 🏗️ Workflow Logic
1.  **Webhook:** Receives incoming messages from platforms like WhatsApp, Facebook, or a Website.
2.  **Filter:** Validates the incoming data to ensure smooth processing.
3.  **AI Agent (Core):**
    * **Memory:** Keeps track of the conversation flow.
    * **Get Services Data:** A tool that allows the AI to "read" what services are available.
    * **Booking Tool:** Appends lead info to Google Sheets.
    * **Calendar Tool:** Creates a live event in Google Calendar once a meeting is confirmed.
4.  **Response:** Sends the final AI-generated message back to the user via Webhook.

---

## 🚀 How to Setup
1.  **Clone the Repository:** Download the `workflow.json` file.
2.  **Import to n8n:** Create a new workflow in n8n and import the JSON file.
3.  **API Keys:** * Add your **Google AI Studio** API key for Gemini.
    * Connect your **Google Console** credentials for Sheets and Calendar.
4.  **Activate:** Save and toggle the workflow to "Active".

---

## 🎯 Use Case: SmartFlow Automations
The agent is programmed with a specific system prompt to:
* Greet users with "Assalamu Alaikum/Namaskar".
* Explain services like WhatsApp/Facebook Automation.
* Redirect pricing queries to a "Free Discovery Meeting."
* Collect leads and confirm bookings instantly.

---
**Developed by [Rabbi Hasan]** *Passionate about AI, No-code Automation, and Workflow Optimization.*
