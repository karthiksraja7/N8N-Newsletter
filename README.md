# 📰 Automated Newsletter with n8n

An automated newsletter workflow built with **n8n** that fetches the latest news from RSS feeds and delivers it to subscribers via **Email** and **Telegram** — fully hands-free.

---

## 🚀 Features

- 📡 Fetches latest news automatically from RSS / API sources
- 📧 Sends formatted newsletter via Email (Gmail / SMTP)
- 💬 Delivers news updates to a Telegram Bot
- ⏰ Scheduled to run automatically at set intervals
- ⚡ No coding required to run — fully managed in n8n

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| [n8n](https://n8n.io) | Workflow automation platform |
| RSS Feed | News data source |
| Gmail / SMTP | Email delivery |
| Telegram Bot API | Telegram message delivery |

---

## 📋 Prerequisites

Before running this workflow, make sure you have:

- [ ] n8n installed ([cloud](https://app.n8n.cloud) or [self-hosted](https://docs.n8n.io/hosting/))
- [ ] A Gmail account with App Password enabled **or** SMTP credentials
- [ ] A Telegram Bot Token (create one via [@BotFather](https://t.me/BotFather))
- [ ] Your Telegram Chat ID

---

## ⚙️ Setup & Installation

### 1. Clone this repository
```bash
git clone https://github.com/your-username/newsletter-n8n.git
cd newsletter-n8n
```

### 2. Import the workflow into n8n
1. Open your n8n instance
2. Go to **Workflows** → **Import from File**
3. Select the `workflow.json` file from this repo

### 3. Configure credentials
Set up the following credentials in n8n (**Settings → Credentials**):

- **Gmail / SMTP** — Add your email and app password
- **Telegram Bot** — Add your Bot Token and Chat ID

### 4. Update RSS Feed URL
In the workflow, open the **RSS Feed node** and replace the URL with your preferred news source.

### 5. Activate the workflow
Toggle the workflow to **Active** — it will now run on schedule automatically.

---

## 📁 Project Structure

```
newsletter-n8n/
├── workflow.json       # n8n workflow export file
└── README.md           # Project documentation
```

---

## 📸 Workflow Preview

> _Add a screenshot of your n8n workflow canvas here_

---

## 🔧 Customization

- **Change schedule** — Edit the Schedule Trigger node to change frequency
- **Add more RSS sources** — Duplicate the RSS node and merge outputs
- **Change email template** — Edit the Gmail node message body
- **Add more Telegram channels** — Duplicate the Telegram node with a different Chat ID

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 🙋‍♂️ Author

Made with ❤️ using [n8n](https://n8n.io)
