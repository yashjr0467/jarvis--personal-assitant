# Jarvis Calendar Agent

> Specialist AI agent that creates Google Calendar events and retrieves events for a requested time range.

**Technologies:** n8n · AI Agent · Google Gemini · Google Calendar

## Overview
This repository contains a sanitized n8n workflow export and setup notes for portfolio review.

## Workflow outline
This workflow uses agent, executeWorkflowTrigger, googleCalendarTool, lmChatGoogleGemini nodes to support the purpose described above. Review the node configuration and connect your own service credentials after import.

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
- calendar agent
- Google Gemini Chat Model
- Create an event in Google Calendar
- Get many events in Google Calendar
- When Executed by Another Workflow

## License
Add a license only if you are comfortable granting others permission to reuse this work.
