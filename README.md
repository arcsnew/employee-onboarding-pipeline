# employee-onboarding-pipeline
n8n HR automation — Greenhouse to Workday to Slack

Employee Onboarding Pipeline
Tools: n8n · Greenhouse · Workday · Slack · Google Sheets

The Problem
Every new hire triggered 3+ hours of manual HR tasks — Workday record creation, Slack welcome message, onboarding tracker update. Steps were often missed or delayed.

The Solution
Built a single n8n workflow triggered the moment a candidate is marked hired in Greenhouse:

Step 1: Webhook fires instantly
Step 2: Extract hire details (name, role, start date, manager)
Step 3: Auto-create Workday employee record via API
Step 4: Send personalised Slack welcome to team channel
Step 5: Add row to Google Sheets onboarding tracker
Step 6: Confirm to HR manager
Error handling: Immediate Slack alert to HR lead if any step fails

## Results
- ⏱️ Time per hire: 3 hours → 0 minutes
- ✅ Manual tasks eliminated: 4 per hire
- 💬 Slack welcome missed: Never
- 📊 Tracker accuracy: 80% → 100%

- Tools Used
n8n — workflow orchestration
Greenhouse — ATS trigger via webhook
Workday — employee record creation via API
Slack — team welcome message
Google Sheets — onboarding tracker
