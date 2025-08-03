# 🧠 Project Architecture – HackerNews Scraper Mailer (Python)

This tool follows a modular Python-based architecture for scraping and emailing Hacker News headlines.

---

## 📊 Overview

The project performs 4 major steps:

1. **Extract Web Page Content**
   - Use `requests` to perform a `GET` request to Hacker News front page.
   - Fetch raw HTML.

2. **Scrape Required Data**
   - Use `BeautifulSoup` to parse HTML.
   - Extract:
     - 📰 Title
     - 🔗 Link
     - ⚡ Score
     - 🌐 Domain Name

3. **Build Email Content**
   - Structure scraped items into readable HTML or plain text.
   - Format: Title → Link → Score

4. **Authenticate & Send Email**
   - Use `smtplib` and Gmail SMTP server.
   - Authenticate with Gmail credentials (use `.env` for security).
   - Compose and send the email using the structured body.

---

## 🧱 Stack Used

| Component       | Tool / Package     |
|----------------|--------------------|
| HTTP Requests   | `requests`          |
| HTML Parsing    | `beautifulsoup4`    |
| Email Sending   | `smtplib`, `email`  |
| Secrets Mgmt    | `python-dotenv`     |

---

## 🔄 Optional Extension

- Use `cron` or Task Scheduler to send this email daily.
- Save logs or output to a `.log` file.



**Packages Used:**

**requests**: For making HTTP requests ✅ (needs to be installed)

**beautifulsoup4**: For web scraping ✅ (needs to be installed)

**smtplib, email.mime, datetime**: For emails and date/time handling ✅ (built into Python)

**smtplib**
It’s a built-in Python library used to send emails using the Simple Mail Transfer Protocol (SMTP).

You use it to connect to an email server (like Gmail’s SMTP server), authenticate, and send email messages from your Python script.

**📄 email.mime**

Part of Python’s email package used to create the structure of email messages.

It helps build email components like the body, attachments, HTML content, and setting headers.

email.mime modules (like MIMEText, MIMEBase) let you format emails properly so that email clients can read them.


## 🔐 Security Note

Always store email credentials in a `.env` file and **never commit it to GitHub**.

