Gmail Automation with CrewAI 📧✨

Intelligent Gmail Inbox Automation Powered by AI Agents

Overview

Gmail Automation with CrewAI is an AI-powered system that automatically manages your Gmail inbox using intelligent agents.

It can:

Categorize incoming emails

Label and prioritize messages

Generate draft replies

Clean up low-value emails

Notify you on Slack for high-priority messages

Powered by CrewAI’s autonomous agent framework, it helps you automate repetitive inbox tasks while maintaining context in email threads.
GitHub Repository

Features

Email Categorization: Classify emails into newsletters, promotions, personal, etc.

Priority Assignment: Assign HIGH/MEDIUM/LOW priority automatically.

Smart Labeling: Apply Gmail labels and stars based on rules.

AI Draft Responses: Generate context-aware reply drafts.

Slack Alerts (Optional): Notify on high-priority messages.

Inbox Cleanup: Automatically delete/archive emails based on rules.

Thread Awareness: Maintain conversation context when processing messages.

Installation

Clone the repository and install dependencies:

git clone https://github.com/softbusinesss/crewai-gmail-automation.git
cd crewai-gmail-automation

# Create a virtual environment
python -m venv .venv
# macOS/Linux
source .venv/bin/activate
# Windows
.\.venv\Scripts\activate

# Install CrewAI dependencies
crewai install


CrewAI framework is required to run the automation.
CrewAI GitHub

Configuration

Create a .env file in the project root:

# LLM Provider
MODEL=openai/gpt-4o-mini
OPENAI_API_KEY=your_openai_api_key

# Gmail Account
EMAIL_ADDRESS=your_email@gmail.com
APP_PASSWORD=your_gmail_app_password

# Optional Slack Webhook
SLACK_WEBHOOK_URL=your_slack_webhook_url


Notes:

Gmail requires an App Password if 2-Step Verification is enabled.

Slack Webhook is optional for alert notifications.

How It Works

Connects securely to Gmail via IMAP.

Reads unread emails.

Categorizes emails and assigns priority.

Applies labels and stars.

Generates AI-based draft replies.

Sends Slack notifications for urgent emails.

Cleans up old, low-priority messages and empties Trash.

Credentials remain local in .env and are never shared externally.

Usage

Run the automation:

crewai run


The system will process unread emails according to your configuration, label and prioritize them, draft replies, notify Slack (if configured), and clean up low-priority messages.

Special Features

Smart Cleanup Rules: Delete promotions > 2 days old, newsletters > 7 days old (unless HIGH priority).

YouTube Email Protection: Keep YouTube notifications marked as read-only.

Context-Aware Drafting: Draft replies preserve email tone and thread context.

Creative Slack Alerts: Alerts for urgent messages with friendly formatting.

Contributing

Contributions are welcome! You can:

Fix bugs or improve automation logic

Add new email handling rules

Improve documentation

Submit changes via Pull Requests on GitHub.

License

MIT License — see the LICENSE file for details.
Repository Link
