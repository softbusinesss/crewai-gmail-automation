Gmail Automation with CrewAI 📧✨

Intelligent Gmail Inbox Automation Powered by AI Agents

🌟 Overview

Gmail Automation with CrewAI is an AI‑driven system that automatically manages your Gmail inbox using intelligent agents. It categorizes incoming emails, labels and prioritizes them, drafts replies, handles cleanup, and can even notify you on Slack — all powered by CrewAI’s autonomous agent framework.

This project uses IMAP to securely access your Gmail account and apply organizational workflows without downloading mail locally.

📌 Table of Contents

✨ Features

🚀 Installation

⚙️ Configuration

📧 How It Works

▶️ Usage

🌟 Special Features

🤝 Contributing

📜 License

✨ Features

📋 Email Categorization: Classifies emails into types like newsletters, promotions, and personal.

🔔 Priority Assignment: Uses rules to assign HIGH/MEDIUM/LOW priority.

🏷️ Smart Labeling: Applies Gmail labels & stars based on content.

💬 AI Draft Responses: Generates reply drafts for key messages.

📱 Slack Alerts: Optional notifications for high‑priority emails.

🧹 Inbox Cleanup: Automatically deletes or archives emails based on rules.

🧵 Thread Awareness: Maintains context within conversation threads.

🚀 Installation

Clone the repository and install dependencies:

git clone https://github.com/softbusinesss/crewai-gmail-automation.git
cd crewai-gmail-automation

# Create and activate a virtual environment
python -m venv .venv
source .venv/bin/activate   # macOS/Linux
.\.venv\Scripts\activate    # Windows

# Install dependencies via CrewAI
crewai install


This project depends on the CrewAI framework for running agent automations.

⚙️ Configuration

Create a .env file in the project root with the following environment variables:

# Choose your LLM provider
# OpenAI (Recommended)
MODEL=openai/gpt-4o-mini
OPENAI_API_KEY=your_openai_api_key

# Or Gemini
# MODEL=gemini/gemini-2.0-flash
# GEMINI_API_KEY=your_gemini_api_key

# Gmail account credentials
EMAIL_ADDRESS=your_email@gmail.com
APP_PASSWORD=your_gmail_app_password

# Optional: Slack webhook URL
SLACK_WEBHOOK_URL=your_slack_webhook_url

🔐 Notes

Gmail requires an App Password for secure access when 2‑Step Verification is enabled.

Slack Webhooks must be created from your Slack workspace if you want alert notifications.

📧 How It Works

This tool uses IMAP to connect securely to your Gmail account:

Secure SSL Connection to Gmail’s IMAP server.

Authenticate with your email and app password.

Mailbox Access to read, label, draft responses, and move messages.

Disconnect Securely after operations complete.

Credentials are stored locally in .env and never shared externally.

▶️ Usage

Run the automation:

crewai run


You’ll be prompted to specify how many unread emails to process (e.g., default 5). The system will:

Fetch unread messages

Categorize by type and priority

Apply labels & stars

Generate draft replies

Send Slack notifications (if configured)

Clean up older, low‑priority emails

Empty Trash to free storage

🌟 Special Features

🎯 Smart Cleanup Rules

Promotions older than 2 days → Deleted

Newsletters older than 7 days (unless HIGH priority) → Deleted

Shutterfly emails → Always deleted

Receipts / documents → Archived

📺 YouTube Email Protection

All YouTube‑related emails are preserved and marked read only — you respond directly on YouTube if needed.

✍️ Smart, Context‑Aware Drafting

Generated replies use email context and grammar suited to message tone.

📣 Creative Slack Alerts

Fun, engaging Slack messages notify you of urgent emails requiring attention.

🧵 Thread Awareness

Maintains message thread context when labeling or drafting replies.

🤝 Contributing

Contributions are welcome! Feel free to:

Fix bugs

Improve rules and prioritization logic

Add new automation behaviors

Improve documentation

Submit your changes via Pull Requests on GitHub.

📜 License

This project is licensed under the MIT License — see the LICENSE file for details.

<p align="center"> <a href="https://github.com/softbusinesss/crewai-gmail-automation"> <img src="https://mintlify.s3.us‑west‑1.amazonaws.com/brightdata/logo/light.svg" width="200" alt="Gmail Automation with CrewAI"> </a> </p>
