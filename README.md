# AI Agent Content Creator

This project is an AI content creator workflow built with n8n.

It reads YouTube URLs from Google Sheets, extracts the transcript, sends it to Groq AI, generates Instagram captions, hashtags, and summaries, then updates the Google Sheet and marks the task as Completed.

## Tools Used

- n8n
- Google Sheets
- Supadata API
- Groq AI
- HTTP Request node

## Future Enhancements

### Instagram Auto Posting

Future versions of this project will:

- Connect to Instagram Graph API
- Automatically publish posts at scheduled times
- Update posting status in Google Sheets

Planned workflow:

Google Sheets → Transcript Extraction → AI Content Generation → Wait Until Scheduled Time → Instagram Graph API → Publish Post → Update Status = Posted

## Workflow Screenshot

![Workflow](workflow-screenshot.png)