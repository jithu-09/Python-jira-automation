# 🛠️ Auto-JIRA Issue Creator via Webhook

This is a lightweight Python Flask API that listens for webhook POST requests and automatically creates a JIRA issue **only when the comment body contains `/jira`**.

---

## 📌 What It Does

- Accepts a JSON payload via a `/createJIRA` POST endpoint
- Checks if the incoming comment body is `/jira`
- If matched, creates a new issue in a specified JIRA project using the Atlassian REST API

---

## 🔧 Tech Stack

- **Python 3**
- **Flask** — for building the API
- **Requests** — for making HTTP calls to the JIRA API
- **python-dotenv** — to load credentials securely from a `.env` file
- **JIRA Cloud API** — to create issues programmatically

---

## 🔐 Authentication

JIRA issue creation uses **Basic Auth** with your Atlassian email and API token.

---

## 💡 Use Cases

- Automate issue creation from GitHub webhooks or bots
- Internal tools that need to log bugs/tasks directly to JIRA
- ChatOps workflows (e.g., Slack slash commands)

---

## 📜 License

MIT — feel free to use and modify!
