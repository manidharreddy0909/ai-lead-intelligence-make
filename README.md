🚀 AI Lead Intelligence Automation (Make + AI)
📌 Overview

This project is a production-style AI-powered lead intelligence automation built using Make (Integromat), OpenAI, Google Forms, Google Sheets, and Gmail.

It automatically:

Captures incoming business inquiries

Understands lead intent using AI

Scores and categorizes leads (Hot / Warm / Cold)

Routes leads into different workflows

Sends automated email responses

Stores structured data for tracking and follow-ups

This is not a demo flow — it reflects how real AI automations are designed and deployed.

🎯 Problem

Most lead-handling systems suffer from:

Manual review of leads

No prioritization

Delayed responses

Missed high-intent prospects

Sales teams waste time on low-quality leads while urgent ones wait.

✅ Solution

An AI-first automation pipeline that:

Collects leads automatically

Uses AI to analyze intent & urgency

Assigns a numeric lead score (0–100)

Categorizes leads as Hot / Warm / Cold

Triggers different actions based on category

All actions happen without human intervention.

🧠 High-Level Architecture

📂 Detailed system design:
➡️ architecture/system-design.md

Core components:

Google Form (Lead Intake)

Make Scenario (Orchestration)

AI Model (Decision Engine)

Google Sheets (Storage)

Gmail (Notifications)

🔄 Workflow Overview

This single workflow handles input → AI reasoning → routing → output.

📥 Lead Input (Google Form)

Leads are captured using a Google Form with structured fields:

Name

Email

Company

Requirement / Message

🤖 AI Lead Analysis

The AI model analyzes each lead and returns structured JSON only:

Intent

Urgency (Low / Medium / High)

Lead score (0–100)

Category (Hot / Warm / Cold)

Prompt design and validation ensure reliable automation.

📂 Prompt details:
➡️ prompts/ai_prompt.md

🔀 Intelligent Routing Logic

Based on AI output:

🔥 Hot leads → Immediate email + priority storage

🌤 Warm leads → Follow-up workflows

❄ Cold leads → Logged for nurturing

This routing is implemented using conditional routers inside Make.

📤 Output & Storage (Google Sheets + Gmail)

Each processed lead is:

Stored in Google Sheets with AI metadata

Automatically emailed with a contextual response

🧪 Testing & Validation

The workflow includes:

Input validation

AI output schema checks

Category & score enforcement

📂 Test cases:
➡️ evaluation/tests.md

🛠️ Setup & Reproducibility

Step-by-step setup instructions are documented.

📂 Setup guide:
➡️ setup/make-setup-guide.md

🔧 Tech Stack

Make (Integromat)

OpenAI (LLM)

Google Forms

Google Sheets

Gmail

💡 Key Learnings

AI as a decision engine, not a chatbot

Structured AI outputs for reliability

Scalable automation design

Real-world lead intelligence workflows

🚀 Future Enhancements

CRM integration (HubSpot / Salesforce)

AI-generated reply personalization

Analytics dashboard

Multi-language lead analysis

📂 Repository Structure
ai-lead-intelligence-make/
├── README.md
├── architecture/
│   └── system-design.md
├── prompts/
│   └── ai_prompt.md
├── setup/
│   └── make-setup-guide.md
├── demo/
│   └── usage.md
├── evaluation/
│   └── tests.md
├── screenshots/
│   ├── workflow-overview.png
│   ├── form-input.png
│   ├── ai-decision.png
│   ├── sheet-output.png
│   └── email-output.png

📌 Why This Project Matters

This project demonstrates:

Real-world AI automation thinking

End-to-end system design

Clean documentation

Business-ready workflows

✅ 2️⃣ FINAL SCREENSHOTS — WHAT TO KEEP / ADD / SKIP
✅ KEEP (You already have most of these)

✔ Workflow canvas (zoomed out)
✔ AI prompt configuration
✔ Google Form structure
✔ Google Sheet with AI columns
✔ Email sent successfully

🖼️ FINAL screenshots/ FOLDER (THIS IS PERFECT)
screenshots/
├── workflow-overview.png   ✅ (zoomed out Make scenario)
├── form-input.png          ✅ (Google Form fields only)
├── ai-decision.png         ✅ (OpenAI prompt + response)
├── sheet-output.png        ✅ (Sheet with AI score/category)
└── email-output.png        ✅ (Successful sent email)
