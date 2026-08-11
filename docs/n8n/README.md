# n8n Workflow

This directory contains the n8n workflows used by the Performance Engineering News Agent.

## Current Workflow

The initial proof-of-concept workflow demonstrates:

```text
Manual Trigger
      ↓
Edit Fields
      ↓
Basic LLM Chain
      ↓
Google Gemini
      ↓
Generated LinkedIn Content
The current workflow is intentionally simple.
It is the starting point for a larger automation pipeline that will eventually:
Monitor trusted performance engineering sources
Identify relevant content
Remove duplicate articles
Score content using AI
Extract technical insights
Generate original LinkedIn content
Publish selected posts automatically
Maintain processing history
Local Development
The n8n environment is currently self-hosted locally using Docker.
The local instance runs on:
http://localhost:5678
Security
Exported workflows must be reviewed before being committed to this repository.
API keys, credentials, tokens, cookies, and other secrets must never be committed to GitHub.
