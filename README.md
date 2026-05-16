# AI Lead Automation CRM

An end-to-end AI-powered lead management automation system built with **n8n**, **Google Forms**, **Google Sheets**, **OpenRouter AI**, **Notion**, and **Gmail**.

The system captures new leads, analyzes them using AI, stores them inside a Notion CRM, and sends automated follow-up emails based on the lead status.

---

## Project Overview

Businesses often receive leads from forms, emails, or landing pages, but manually reviewing, scoring, organizing, and following up with each lead takes time.

This project automates the full lead management process:

1. Capture lead information from a Google Form
2. Store responses in Google Sheets
3. Trigger an n8n workflow when a new row is added
4. Send lead data to an AI model using OpenRouter API
5. Classify the lead as Hot, Warm, or Cold
6. Save the lead and AI analysis inside Notion CRM
7. Send an automated follow-up email using Gmail

---

## Workflow Architecture

```text
Google Form
    ↓
Google Sheets
    ↓
n8n Google Sheets Trigger
    ↓
OpenRouter AI API
    ↓
JavaScript Code Node
    ↓
Notion CRM
    ↓
IF Lead Status
    ↓
Gmail Follow-up Email
