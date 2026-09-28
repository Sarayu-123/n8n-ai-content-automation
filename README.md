# 🤖 AI Content Generator & Auto Publisher

### ⚡ From topic → AI-generated article → WordPress → social-ready content

An automated content pipeline built with **n8n**, **Ollama**, **Llama 3**, and **WordPress**.

The workflow dynamically selects a topic, generates a complete blog using a **local LLM**, transforms the output into publish-ready HTML, automatically publishes it to WordPress, and generates a social-media-ready post.

---

## ✨ What It Does

```text
🕐 Schedule Trigger
        ↓
🎯 Dynamic Topic Generation
        ↓
🧠 Ollama + Llama 3
        ↓
✍️ Blog Generation
        ↓
⚙️ JavaScript Formatting
        ↓
🌐 WordPress Publishing
        ↓
📱 Social Post Generation

🚀 Features
🕐 Scheduled Automation — Automatically triggers the workflow
🎯 Dynamic Topics — Selects topics programmatically
🧠 Local AI Generation — Uses Ollama with Llama 3
✍️ Content Processing — Extracts and structures generated content
⚙️ JavaScript Formatting — Converts AI output into publish-ready HTML
🌐 Auto Publishing — Creates and publishes WordPress posts
📱 Social Content — Generates social-media-ready summaries
🔒 Local AI — Content generation runs locally
🧩 Tech Stack
Technology	Purpose
n8n	Workflow automation
Ollama	Local LLM runtime
Llama 3	AI content generation
WordPress	Blog publishing
JavaScript	Content processing and formatting
REST APIs	Service communication
XAMPP	Local WordPress environment
🔄 Workflow Breakdown
1. 🕐 Schedule Trigger

Starts the automation according to the configured schedule.

2. 🎯 Dynamic Topic Generation

A JavaScript expression selects a topic from the predefined topic set.

3. 🧠 AI Content Generation

n8n sends the selected topic to Ollama running Llama 3, which generates a structured blog article containing:

Title
Introduction
Multiple sections
Conclusion
4. ⚙️ Content Formatting

JavaScript processes the generated response and converts the Markdown-style structure into HTML suitable for WordPress.

5. 🌐 WordPress Publishing

The formatted article is sent through the WordPress integration and published automatically.

6. 📱 Social Post Generation

A final JavaScript node creates a short social-media-ready version of the generated article.

🏗️ Architecture
              ┌───────────────────┐
              │  🕐 Schedule      │
              │     Trigger       │
              └─────────┬─────────┘
                        ↓
              ┌───────────────────┐
              │  🎯 Topic         │
              │     Generator     │
              └─────────┬─────────┘
                        ↓
              ┌───────────────────┐
              │  🧠 Ollama        │
              │     Llama 3       │
              └─────────┬─────────┘
                        ↓
              ┌───────────────────┐
              │  ⚙️ JavaScript    │
              │     Formatter     │
              └─────────┬─────────┘
                        ↓
              ┌───────────────────┐
              │  🌐 WordPress     │
              │     Publisher     │
              └─────────┬─────────┘
                        ↓
              ┌───────────────────┐
              │  📱 Social Post   │
              │     Generator     │
              └───────────────────┘
💡 Key Highlights
🔗 End-to-end workflow automation
🧠 Local LLM integration using Ollama
🔌 HTTP / REST API integration
⚙️ JavaScript-based data transformation
🌐 Automated WordPress publishing
🔄 Dynamic and repeatable content pipeline
🔒 No external AI API required for content generation
📁 Project Structure
n8n-ai-content-automation/
│
├── myworkflow.json    # Exported n8n workflow
├── README.md          # Project documentation
└── .gitignore         # Git ignore rules
🛠️ Run Locally
Prerequisites
Node.js
n8n
Ollama
Llama 3
WordPress
XAMPP
Start n8n
npx n8n

Then open:

http://localhost:5678

Import myworkflow.json, configure the required WordPress credential, and run the workflow.

🔐 Local & Security Notes

This repository contains the workflow definition and documentation only.

The following remain local and are not committed:

n8n local database
n8n credentials
WordPress installation and database
Ollama model files
Environment variables
Passwords and API credentials
🎯 Project Goal

Build a reusable AI-powered content automation pipeline that reduces manual effort across:

Topic Selection → Content Creation → Formatting → Publishing → Social Content

👩‍💻 Author

N. Ch. Sarayu

Computer Science Engineering | AI & ML

GitHub
