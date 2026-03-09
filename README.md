# AI Client Onboarding Automation

An AI-powered onboarding workflow built in n8n that validates incoming form submissions, creates or updates CRM contacts, sends onboarding emails, and notifies internal teams.

This workflow demonstrates event-driven automation, CRM integration, delayed onboarding sequences, and multi-channel notifications.

---

## Features

- Triggered by new form submissions
- Validates required onboarding data
- Creates and updates contact records in HubSpot
- Sends internal team notifications
- Sends automated welcome and follow-up emails
- Downloads and sends onboarding guide materials
- Uses wait steps for staged onboarding communication

---

## Workflow Architecture

JotForm Trigger  
→ Validate required fields  
→ Create CRM contact  
→ Notify internal team  
→ Send welcome email  
→ Wait  
→ Download onboarding guide  
→ Send onboarding guide email  
→ Wait  
→ Send offer email  
→ Update CRM status  
→ Final onboarding confirmation  
→ Notify internal team

---

## Tech Stack

- n8n
- JotForm
- HubSpot API
- Gmail API
- Telegram API
- Google Drive API

---

## Example Use Case

When a new customer submits an onboarding form, the workflow:

1. validates the submission
2. creates a CRM contact
3. alerts the internal team
4. sends a welcome email
5. follows up with onboarding materials
6. updates lifecycle status over time

This reduces manual onboarding work and ensures a consistent customer experience.

---

## Files

- `workflow/client-onboarding-workflow.json`
- `sample-data/sample-form-submission.json`

---

## Workflow Diagram

![Workflow](screenshots/workflow-diagram.png)

---

## Setup Instructions

1. Import the workflow JSON into n8n.
2. Connect your credentials for:
   - JotForm
   - HubSpot
   - Gmail
   - Telegram
   - Google Drive
3. Replace all placeholder values with your own configuration.
4. Activate the workflow.

---

## Security

All credentials, IDs, links, and private identifiers have been removed from this repository.
