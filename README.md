<p align="center"> <a href="https://github.com/softbusinesss/crewai-gmail-automation"> <img src="https://mintlify.s3.us-west-1.amazonaws.com/brightdata/logo/light.svg" width="300" alt="Gmail Automation with CrewAI"> </a> </p>
Gmail Automation with CrewAI ✨

AI‑Powered Email Management & Workflow Automation System
An intelligent, multi‑agent system that uses CrewAI to automatically categorize, organize, respond to, and clean up your Gmail inbox.

<div align="center"> <img src="https://img.shields.io/badge/python‑AI‑automation‑blue"/> <img src="https://img.shields.io/badge/License‑MIT‑blue"/> </div>
🌟 Overview

This project is a smart Gmail automation tool leveraging AI agents to:

Categorize incoming emails (newsletters, promotions, personal, etc.)

Assign priority levels (HIGH, MEDIUM, LOW)

Apply Gmail labels & stars

Generate intelligent draft responses

Send notifications to Slack for high‑priority items

Clean up low‑value emails

Maintain thread awareness and email context

Powered by CrewAI’s agent framework, this system helps you automate repetitive inbox tasks and stay on top of important messages.

📌 Table of Contents

✨ Features

🛠 Installation

⚙️ Configuration

📧 How It Works

▶️ Usage

🔍 Special Features

🤝 Contributing

📜 License

✨ Features

📋 Email Categorization — Classifies emails by type

🔔 Priority Assignment — Intelligent scoring of message importance

🏷️ Smart Organization — Apply Gmail labels & stars based on rules

💬 AI‑Generated Drafts — Context‑aware reply drafts

📱 Slack Notifications — Alerts for high‑priority messages

🧹 Cleanup Automation — Delete low‑priority emails with safe rules

🧵 Thread Awareness — Maintains conversation structure

🛠 Installation

Clone the repository:

git clone https://github.com/softbusinesss/crewai-gmail-automation.git
cd crewai-gmail-automation


Create and activate a virtual environment:

python -m venv .venv
source .venv/bin/activate   # macOS/Linux
.\.venv\Scripts\activate    # Windows


Install dependencies via CrewAI:

crewai install

⚙️ Configuration

Create a .env file in the project root with:

# LLM provider settings
MODEL=openai/gpt-4o-mini
OPENAI_API_KEY=your_openai_api_key

# Gmail account credentials
EMAIL_ADDRESS=your_email@gmail.com
APP_PASSWORD=your_gmail_app_password

# Optional: Slack notifications
SLACK_WEBHOOK_URL=your_slack_webhook_url


💡 Notes:

Gmail requires 2‑Step Verification and an App Password for IMAP access.

Slack Webhook setup is optional but enables alerting for priority messages.

📧 How It Works

This tool uses IMAP (Secure Mail Access) to connect to your Gmail inbox and perform actions such as:

Fetch unread emails

Categorize and assign labels

Generate draft replies using AI

Send Slack alerts for critical messages

Delete or archive emails based on customizable rules

The connection is secure, and credentials remain local in .env — never shared externally.

▶️ Usage

Run the automation with:

crewai run


You’ll be prompted for how many emails to process. The script will then:

Fetch unread messages

Categorize them

Apply labels & stars

Generate draft replies

Send Slack notifications

Clean up older, lower‑priority emails

Empty trash to free space

🔍 Special Features

🗓️ Smart Cleanup Rules:

Delete promotions > 2 days old

Delete newsletters > 7 days old (unless high priority)

Always remove certain categories like Shutterfly

Archive receipts & important documents instead of deleting

🎬 YouTube Email Protection:

Preserves YouTube‑related notifications and marks them as READ_ONLY

✍️ AI Draft Replies:

Tailored to the message context with proper grammar & formatting

🎨 Creative Slack Alerts:

Fun and informative notifications for urgent emails

🧵 Thread Handling:

Keeps responses and actions context‑aware within threads

🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request with:

New automation features

Bug fixes & improvements

Enhanced machine learning rules

Updated documentation

📜 License

This project is licensed under the MIT License — see the LICENSE file for details.

<p align="center"> <a href="https://github.com/softbusinesss/crewai-gmail-automation"> <img src="https://mintlify.s3.us-west-1.amazonaws.com/brightdata/logo/light.svg" width="200" alt="Gmail Automation with CrewAI"> </a> </p>
