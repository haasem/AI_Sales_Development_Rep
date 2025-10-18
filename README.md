🧠 AI Workflow Automation: Lead Qualifier + Voice Agent
Source: Google Sheets + n8n + GPT + VAPI + Slack + Gmail + Google Drive Integration
🌍 Overview

This project demonstrates an end-to-end AI-driven business workflow that automates lead qualification, voice outreach, and proposal generation.
Built with n8n, the system connects multiple business tools — Google Sheets, OpenAI, VAPI (Voice AI), Gmail, Slack, and Google Drive — into a single autonomous process that handles leads from intake to proposal delivery without manual effort.

The goal: to streamline lead engagement for small and mid-sized agencies by replacing repetitive sales admin work with intelligent automation and conversational AI.

<img width="1296" height="470" alt="image" src="https://github.com/user-attachments/assets/45ed378c-e80c-4842-9fa6-11fa251e73ed" />


🧩 Workflow Summary

1. Lead Intake via Google Sheets

When a new lead fills out a contact form, their details are automatically logged in a connected Google Sheet (e.g., through Tally or other form systems).
n8n detects the new entry and triggers the workflow.


2. Company Research & Personalization (AI-powered)

Before any contact occurs, the system calls OpenAI GPT to analyze the company’s name and notes, summarizing:
- What the company does
- Its likely challenges or goals
- How AI automation could help

This research summary is used to personalize the voice conversation with the lead.


3. Voice Agent Outreach (via VAPI.ai)

The workflow then activates a Voice AI Agent (using VAPI.ai) that calls the lead directly.
During the call, the AI assistant:
- Greets the lead by name
- Explains the agency’s AI automation services
- Asks targeted discovery questions
- Determines whether the lead is interested in receiving a proposal

All conversations are recorded and transcribed, and a summary of the discussion is automatically returned to the workflow.


4. Automated Qualification & Follow-up

Depending on the call result:
✅ Interested leads → Update Google Sheet, mark as Contacted & Interested
❌ Unsuccessful calls → Send a follow-up email with a Calendly link and notify the marketing team on Slack

This ensures no lead goes uncontacted while maintaining a professional, consistent follow-up flow.


5. AI-Generated Proposal Creation

If the lead shows interest, a second AI process generates a proposal draft using GPT.
The system decides automatically whether to recommend:
- AI Automation Services
- AI Agent Deployment
- or Both, based on the conversation context.

The proposal includes:
- A summary of client goals
- Recommended services
- Implementation outline
- Itemized pricing & total cost

This information is merged into a Google Docs template, exported as a PDF, and saved in the “Proposals” folder on Google Drive.


6. Proposal Delivery

Finally, the PDF proposal is automatically emailed to the lead via Gmail, and the status in Google Sheets is updated to mark the proposal as sent.

⚙️ Tech Stack & Integrations
Component	Purpose
- n8n	Central workflow automation platform orchestrating all steps
- Google Sheets	Lead data source and CRM-like tracking sheet
- OpenAI GPT-4.1-mini	Used for company research, reasoning, and proposal generation
- VAPI.ai	Provides the conversational AI voice agent
- Gmail	Handles automated email communications (to leads and internal teams)
- Slack	Sends notifications to marketing and sales channels
- Google Drive + Docs	Hosts proposal templates and stores generated documents


🧠 Business Value

This project demonstrates how AI agents and workflow automation can eliminate friction in early-stage customer engagement.
It shows the ability to:
- Combine data, communication, and AI reasoning across tools
- Design autonomous sales processes that feel personal and intelligent
- Deliver real business ROI by saving time and reducing lead response delays

For recruiters, CTOs, or business sponsors, this project highlights a blend of business understanding, technical design, and automation strategy — bridging the gap between operational efficiency and intelligent customer experience.


📈 Example Scenario

- A potential client submits a request to learn how AI can optimize their business.
- Within minutes, the AI Voice Agent calls them, holds a natural conversation, and collects their needs.
- The system analyzes the discussion, drafts a customized proposal, and delivers it via email — all within an hour, with no human intervention.


🧰 Skills Demonstrated

- Automation architecture and workflow design (n8n)
- Prompt engineering for business context understanding
- Integration across multiple APIs (Google, OpenAI, Slack, VAPI)
- LLM-driven content generation for structured documents
- Applied AI strategy for sales and marketing operations
