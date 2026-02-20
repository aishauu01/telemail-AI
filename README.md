# telemail-AI
📧 n8n AI Mail Assistant

An intelligent email automation workflow built using n8n, OpenAI, Telegram Bot API, and Gmail API.

This project enables users to manage emails directly from Telegram using natural language. The AI agent can summarize emails, send emails, or perform both tasks and return a structured execution report.

🚀 Features

📩 Summarize Gmail messages

✉️ Send emails using natural language instructions

🔁 Summarize and forward emails

🤖 AI-powered decision-making using OpenAI

📲 Telegram-based interaction interface

📊 Structured execution report output

🔐 Secure credential handling via n8n

🏗️ Architecture Overview

Telegram → n8n Workflow → AI Agent (OpenAI) → Gmail API → Telegram Response

Components Used

Telegram Trigger Node – Receives user messages

OpenAI Chat Model – Interprets user intent

AI Agent Node – Decides task execution

Gmail Tool Node – Fetches or sends emails

Telegram Node – Returns execution report

🛠️ Tech Stack

n8n (Workflow Automation)

OpenAI GPT Model (gpt-5-mini or configurable)

Gmail API (OAuth2)

Telegram Bot API

JavaScript Expressions (within n8n)

📂 Workflow Capabilities

The AI assistant supports three primary operations:

Email Summary

Retrieves emails from Gmail

Generates concise summaries

Email Sending

Sends emails using AI-extracted fields

Supports dynamic subject and message content

Email Summary & Send

Summarizes email content

Sends the summary to a specified recipient

📋 Output Format

The assistant returns a structured execution report:

Task Performed:
Email Summary / Email Sent / Email Summary & Sent

Details:
Brief task-specific description

Status:
Success

No additional text, greetings, or explanations are included.

🔧 Setup Instructions
1️⃣ Prerequisites

n8n installed (Cloud or Self-Hosted)

Telegram Bot Token

Gmail OAuth2 Credentials

OpenAI API Key

2️⃣ Import Workflow

Open n8n

Go to Workflows

Click Import

Paste the provided JSON workflow

Save

3️⃣ Configure Credentials

Connect:

Telegram API

Gmail OAuth2

OpenAI API

4️⃣ Activate Workflow

Enable the workflow

Start sending commands via Telegram

💡 Example Commands

“Summarize my latest email”

“Send an email to john@example.com
 about the meeting”

“Summarize the last email and send it to my manager”

🔐 Security Notes

Credentials are not included in the repository.

OAuth2 authentication is required for Gmail access.

Store API keys securely within n8n credential manager.

📈 Use Cases

Email automation for professionals

AI-powered inbox assistant

Low-code LLM orchestration example

Workflow automation portfolio project

👨‍💻 Author

Built using n8n and OpenAI for intelligent workflow automation.
