# AI-News-Intelligence-Summarizer-N8N
AI-powered news intelligence system built with n8n, Google Gemini, RSS feeds, and Gmail. Automatically collects AI news, technology updates, and upcoming AI events, generates concise summaries, and delivers a personalized daily newsletter directly to your inbox.
# 🚀 AI News Intelligence Summarizer

An AI-powered news aggregation and newsletter automation system built using **n8n**, **Google Gemini**, **RSS Feeds**, **SerpAPI**, and **Gmail**.

The workflow automatically collects AI news, technology updates, and upcoming AI events from multiple sources, generates a concise daily intelligence report using Google Gemini, and delivers the summarized newsletter directly to your email inbox.

---

## 📌 Project Overview

Keeping up with rapidly evolving AI and technology news requires visiting multiple websites, reading numerous articles, and filtering relevant information.

This project automates the entire process by:

- Collecting AI news from multiple RSS feeds
- Fetching upcoming AI-related events
- Aggregating news from different sources
- Summarizing content using Google Gemini
- Delivering a personalized daily newsletter via email

Instead of spending 30–45 minutes browsing multiple websites, users receive a curated AI news digest in just a few minutes.

---

## 🎯 Problem Statement

Professionals, developers, researchers, and AI enthusiasts often struggle to:

- Monitor multiple AI news sources
- Track important technology developments
- Stay informed about upcoming AI events
- Consume large volumes of information efficiently

The goal of this project is to provide a centralized AI-powered news intelligence system that delivers only the most relevant information.

---

## ✨ Features

### 📰 Multi-Source News Collection

- Fetches AI news from multiple RSS feeds
- Supports technology and AI news sources
- Collects latest articles automatically

### 📅 AI Event Tracking

- Retrieves upcoming AI and technology events
- Uses SerpAPI Google Events integration
- Includes event information in newsletters

### 🔄 Data Aggregation

- Merges content from multiple sources
- Creates a unified dataset for processing
- Eliminates the need for manual filtering

### 🤖 AI-Powered Summarization

Google Gemini automatically:

- Identifies important news
- Extracts key insights
- Creates concise summaries
- Generates newsletter-ready content

### 📧 Automated Email Delivery

- Sends personalized newsletters
- Delivers updates directly to Gmail
- Runs automatically on schedule

---

## 🏗️ Workflow Architecture

```text
Schedule Trigger
        │
        ▼
 ┌─────────────┬─────────────┬─────────────┐
 │             │             │
 ▼             ▼             ▼

RSS Feed 1   RSS Feed 2   AI Events API
 │             │             │
 └─────────────┴─────────────┘
               │
               ▼

         Data Merger
               │
               ▼

       Data Aggregator
               │
               ▼

     Google Gemini AI
      Summarization
               │
               ▼

        Gmail Sender
               │
               ▼

      Daily Newsletter
```

---

## ⚙️ Workflow Components

### 1️⃣ Schedule Trigger

Automatically starts the workflow every day.

Current Configuration:

```text
10:00 AM Daily
```

---

### 2️⃣ RSS Feed Readers

The workflow collects news from:

#### AI Business

```text
https://aibusiness.com/rss.xml
```

#### NormalTech

```text
https://www.normaltech.ai/feed
```

These feeds provide the latest AI and technology news updates.

---

### 3️⃣ Event Discovery

Uses SerpAPI Google Events Search.

Query:

```text
AI Tech Events in India
```

The workflow gathers:

- Event names
- Dates
- Locations
- Event descriptions

---

### 4️⃣ Data Merger

Combines data from:

- AI News Feed
- Technology Feed
- AI Event Feed

into a single processing pipeline.

---

### 5️⃣ Data Aggregator

Aggregates all collected information into a unified dataset before sending it to Gemini.

---

### 6️⃣ Google Gemini Chat Model

Gemini acts as the intelligence engine.

Responsibilities:

- Analyze collected content
- Filter important information
- Create daily summaries
- Structure newsletter output

Generated Sections:

- AI News Highlights
- Technology Updates
- Upcoming AI Events

---

### 7️⃣ Gmail Sender

Automatically sends the generated newsletter.

Subject:

```text
Today's AI News for you...
```

---

## 🛠️ Technology Stack

| Category | Technology |
|-----------|-----------|
| Workflow Automation | n8n |
| Generative AI | Google Gemini |
| News Source | RSS Feeds |
| Event Discovery | SerpAPI |
| Email Service | Gmail |
| Authentication | OAuth 2.0 |
| Cloud Services | Google Cloud Platform |

---

## 📸 Workflow Screenshot

### Complete Workflow

![Workflow](screenshots/workflow-overview.png)

---

## 📂 Repository Structure

```text
AI-News-Intelligence-Summarizer/
│
├── README.md
├── workflow/
│   └── AI_News_Summarizer_Workflow.json
│
├── screenshots/
│   ├── workflow-overview.png
│   ├── rss-feed-configuration.png
│   ├── gemini-summarization.png
│   ├── generated-newsletter.png
│   └── workflow-execution.png
│
├── docs/
│   └── Project_Documentation.pdf
│
└── assets/
    └── architecture-diagram.png
```

---

## 🎓 Learning Outcomes

Through this project, I gained hands-on experience in:

- Workflow Automation using n8n
- Google Gemini Integration
- RSS Feed Processing
- Data Aggregation Techniques
- Gmail API Integration
- OAuth Authentication
- Prompt Engineering
- AI-Powered Content Summarization
- Automated Newsletter Systems

---

## 🚀 Future Enhancements

- Personalized News Categories
- Slack Integration
- Telegram Notifications
- Weekly Intelligence Reports
- Sentiment Analysis
- Trending Topic Detection
- News Analytics Dashboard
- Multi-Language Summaries

---

## 👨‍💻 Author

**Manish Rana**

Integrated M.Tech in Computer Science & Engineering  
VIT Bhopal University

### Areas of Interest

- Artificial Intelligence
- Machine Learning
- Workflow Automation
- Generative AI
- Data Analytics
- Full Stack Development

---

⭐ If you found this project useful, consider giving it a star!
