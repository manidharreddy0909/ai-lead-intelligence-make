## System Architecture

1. User submits a Google Form
2. Response is stored in Google Sheets
3. Make scenario triggers on new row
4. AI analyzes the message for intent and urgency
5. Output is returned as structured JSON
6. Router classifies lead as Hot, Warm, or Cold
7. Email is sent based on classification
8. CRM fields are updated in the same row
9. Logs are recorded for monitoring

AI is used as a reasoning layer only.
All decisions are enforced by deterministic routing logic.
 
