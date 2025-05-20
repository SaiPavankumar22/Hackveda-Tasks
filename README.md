# 📡 **QueryNotifier** – Smart Keyword Question Notifier

`QueryNotifier` is a Python automation tool that scrapes **user questions from Quora and Reddit** using the Google Custom Search API and **sends the results via email** in CSV format. Ideal for monitoring niche topics like coding competitions, AI trends, or startup discussions, this tool streamlines content discovery and notification delivery.

---

## 🚀 Features

* ✅ User keyword input (e.g., *"Coding Competitions"*)
* 🔍 Scrapes community Q\&A from Quora and Reddit using Google's Programmable Search
* 📦 Saves question titles into a structured `.csv` file
* 📧 Emails the CSV file automatically with a custom message
* 🔧 Easy to customize for other sites, keywords, and recipients

---

## 🧠 Technologies & Tools Used

| Category             | Tools/Technologies                    |
| -------------------- | ------------------------------------- |
| Web Scraping/API     | Google Custom Search API (`requests`) |
| Data Processing      | `pandas`, `json`                      |
| Email Automation     | `smtplib`, `email.mime`, Gmail SMTP   |
| File Format          | CSV                                   |
| Programming Language | Python                                |

---


## ⚙️ Setup Instructions

1. **Clone this repository** or copy the script to your project.

2. **Install Python dependencies**:

   ```bash
   pip install pandas
   ```

3. **Configure Google Programmable Search**:

   * Go to [Programmable Search Engine](https://programmablesearchengine.google.com/)
   * Add `quora.com` and `reddit.com` as searchable sites
   * Get your **API Key** and **Custom Search Engine ID (cx)**

4. **Edit the Script**:

   * Replace `your google api key` and `custom search engine id` in the script
   * Update the sender and receiver emails with your Gmail App Password

5. **Run the script**:

   ```bash
   python queryping.py
   ```

---

## 📬 Example Email Output

* **Subject**: NEW CODING COMPETITIONS
* **Body**:

  ```
  Hello,
  New notifications regarding "CODING COMPETITIONS" are released,
  here I am attaching a file of notifications.
  Thanks,
  D.Sai Pavan
  ```
* **Attachment**: `coding_competitions_questions.csv`

---

## 💡 Use Cases

* 📚 **Academic Research** – Collect public questions on technical or social topics
* 🚨 **Alerts & Monitoring** – Be notified when communities discuss your interests
* 📤 **Team Knowledge Sharing** – Distribute relevant Q\&A topics to your teammates
* 🧠 **Trend Analysis** – Track frequently asked questions over time

---

## 🔐 Security Note

* Use **Gmail App Passwords**, not raw Gmail passwords.
* Keep API keys and email credentials secure using environment variables or `.env` files.

---

## ✍️ Author

**D. Sai Pavan Kumar**
