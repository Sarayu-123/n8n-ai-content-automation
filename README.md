\# AI Content Generator + Auto Publisher



\## Overview



An AI-powered content automation workflow built with n8n.



The workflow automatically generates blog articles using a local LLM through Ollama, formats the generated content, publishes it to WordPress, and generates a social-media-ready post.



\## Workflow



Schedule Trigger

→ Dynamic Topic Generation

→ Ollama AI Generation

→ Blog Extraction

→ JavaScript Formatting

→ WordPress Publishing

→ Social Media Post Generation



\## Features



\- Scheduled content generation

\- Dynamic AI topic selection

\- Local AI content generation using Ollama

\- Blog formatting using JavaScript

\- Automatic WordPress publishing

\- Social-media-ready post generation



\## Technologies



\- n8n

\- Ollama

\- Llama 3

\- WordPress

\- JavaScript

\- REST APIs

\- XAMPP



\## How It Works



1\. The Schedule Trigger starts the workflow.

2\. A topic is selected dynamically.

3\. Ollama generates the blog article using Llama 3.

4\. The generated content is extracted and processed.

5\. JavaScript formats the article for WordPress.

6\. The WordPress node creates and publishes the post.

7\. A JavaScript node generates a social-media-ready version.



\## Local Setup



This project runs locally using:



\- n8n

\- Ollama with Llama 3

\- WordPress

\- XAMPP



Import `workflow/workflow.json` into n8n and configure the required WordPress credentials.



\## Project Structure



```text

n8n-ai-content-automation/

│

├── workflow/

│   └── workflow.json

│

├── README.md

└── .gitignore

Notes



The workflow uses a local Ollama model, so no external AI API is required for content generation.



WordPress is used as the local publishing platform.



Author



N. Ch. Sarayu

