📸 Workflow Screenshots & Visual Walkthrough

This document provides a visual walkthrough of the AI Lead Intelligence Automation built using Make + AI.
Each screenshot corresponds to a specific stage in the automation pipeline.

1️⃣ End-to-End Workflow Overview

This image shows the entire Make scenario, from lead ingestion to AI processing and automated outputs.

2️⃣ Lead Intake – Google Form

Leads are captured using a structured Google Form containing:

Name

Email

Company

Requirement / Message

3️⃣ AI Lead Analysis (Prompt & Reasoning)

The AI model analyzes incoming leads and produces structured output only:

Intent

Urgency

Lead Score (0–100)

Category (Hot / Warm / Cold)

4️⃣ Data Storage – Google Sheets

All processed leads are stored automatically in Google Sheets along with AI-generated metadata.

5️⃣ Automated Email Notification

Based on lead category, an automated email is sent via Gmail without manual intervention.

✅ Notes

Sensitive information (emails, IDs) has been hidden or anonymized.

Screenshots represent real executions of the workflow.

This automation runs fully hands-free once deployed.

🔗 Related Documentation

Main Project Overview: ../README.md

System Design: ../architecture/system-design.md

AI Prompt Design: ../prompts/ai_prompt.md

Setup Guide: ../setup/make-setup-guide.md
