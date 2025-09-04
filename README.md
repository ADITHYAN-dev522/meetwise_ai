# meetwise_ai
**MeetWise AI** turns meetings into actionable results by integrating with Google Calendar . It processes transcripts, summarizes key points, and extracts action items with owners and deadlines. Summaries are shared to Slack or Notion instantly, ensuring follow-ups aren't missed. Built with FastAPI, Streamlit, and AI for quick, real impact.

# MeetWise AI - Smart Meeting Summarizer & Action Tracker

## Overview
MeetWise AI ingests meeting transcripts and automatically:
- Summarizes the meeting.
- Extracts action items (owner + optional deadline).
- Sends summary & actions to Slack and/or Notion.
- Stores summary in a lightweight SQLite DB.

## Quickstart
- Create project directory meetwise-ai and paste files exactly as named.
- cp .env.example .env then fill values.
- Install deps: pip install -r requirements.txt.
- Run server: uvicorn main:app --reload --port 8000.
- Use the /docs OpenAPI UI to exercise endpoints, or call via curl/Postman.

## .env.example
# Descope
DESCOPE_PROJECT_ID=your_descope_project_id
DESCOPE_MANAGEMENT_KEY=your_descope_management_key

# Google
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
GOOGLE_API_KEY=your_google_api_key

# Slack
SLACK_BOT_TOKEN=xoxb-your-bot-token
SLACK_SIGNING_SECRET=your-signing-secret

# Notion
NOTION_API_KEY=your_notion_api_key
NOTION_DATABASE_ID=your_notion_database_id

# OpenAI
OPENAI_API_KEY=your_openai_api_key

# App
APP_ENV=development
APP_PORT=8000
LOG_LEVEL=info

# Database
DATABASE_URL=sqlite:///./meetwise.db


