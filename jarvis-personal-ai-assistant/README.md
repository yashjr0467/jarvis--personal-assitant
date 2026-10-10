# YASH_ai / Jarvis Personal Assistant

> Webhook-based central assistant that routes requests to calendar, email, content-creation, contact, and web-search specialist tools.

**Technologies:** n8n · AI Agent · Google Gemini · Multi-Agent

## Overview
This repository contains a sanitized n8n workflow export and setup notes for portfolio review.

## Specialist tools
- Calendar agent
- Email agent
- Content creator
- Contact agent
- Tavily web search

The main workflow calls other workflows by n8n workflow references. After importing, reconnect each referenced workflow in your own n8n instance and verify the webhook path and request payload before testing.

## Import into n8n
1. Download `workflow.json` from this repository.
2. In n8n, create a workflow or open the workflow menu and choose **Import from File**.
3. Select `workflow.json`.
4. Reconnect required credentials (for example, Google Gemini, Gmail, Google Calendar, Google Contacts, Airtable, Tavily, or Supabase).
5. Review every node's parameters, service permissions, and trigger schedule.
6. Test with synthetic/sample data before enabling the workflow.

## Included files
- `workflow.json` — sanitized n8n workflow export.
- `README.md` — project overview and setup instructions.

## Important notes
- Credentials and webhook IDs have been removed from the export. You must reconnect credentials in your own n8n instance.
- Some integrations require account-specific IDs, schemas, or workflow references to be reconfigured after import.
- The workflow is provided for learning and demonstration. Verify the configuration and behavior in a test environment before production use.
- Do not commit API keys, OAuth tokens, personal data, customer messages, or confidential business information.

## Node inventory
- Webhook
- Google Gemini Chat Model
- Simple Memory
- YASH_ai
- Respond to Webhook
- calendar agent
- Call 'email agent'
- Call 'content_creation'
- Call 'contact agent'
- Search in Tavily

## License
Add a license only if you are comfortable granting others permission to reuse this work.
