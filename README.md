# hackernews-scraper-mailer-py
A Python-based automation tool that scrapes top headlines from Hacker News and emails them to you daily.


This project is a complete Python automation tool that scrapes the latest headlines from the Hacker News front page and delivers them directly to your email inbox. It’s a great example of using Python for web scraping, email automation, and task scheduling.

**It includes**

Web scraping using requests and BeautifulSoup

Email automation using smtplib or third-party email APIs

Secure credentials management using .env files

Project structuring and basic Python packaging

Optional task scheduling via cron (Linux/macOS) or Task Scheduler (Windows)

🔧 **Features**

Scrapes real-time front-page stories from Hacker News

Formats headlines into a neat email layout

Sends daily digest emails automatically

Customizable email recipient, sender, and frequency

Built with pure Python and minimal dependencies

**📦 Tech Stack**

Python 3.x

requests for HTTP requests

BeautifulSoup for HTML parsing

smtplib or email for sending emails

dotenv for secure environment variables

Cron/Task Scheduler for automation (optional)
