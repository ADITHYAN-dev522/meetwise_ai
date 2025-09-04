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


USE THE OFFICAL API KEYS IN THE .env FOR THE PROPER FUNCTIONING OF THE PROJECT OR THE STUBBED DATA WOULD BE SHOWN
LOG_LEVEL=info

# Database
DATABASE_URL=sqlite:///./meetwise.db


