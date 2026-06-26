# AI Agent Content Creator

This project is an AI content creator workflow built with n8n.

It reads YouTube URLs from Google Sheets, extracts the transcript, sends it to Groq AI, generates Instagram captions, hashtags, and summaries, then updates the Google Sheet and marks the task as Completed.

## Tools Used

- n8n
- Google Sheets
- Supadata API
- Groq AI
- HTTP Request node

## Instagram Auto Posting

This project has been extended to support Instagram auto-posting using the Meta Instagram Graph API.

The workflow can:

- Generate Instagram captions using AI
- Use a public image URL for the Instagram post
- Create Instagram media through the Meta Graph API
- Publish the media to Instagram
- Update the posting status in Google Sheets

Workflow:

Google Sheets → Transcript Extraction → AI Content Generation → Wait Until Scheduled Time → Create Instagram Media → Publish Instagram Post → Update Status = Posted

## Instagram Posting Result

After the AI workflow completes, the generated content is automatically published to the connected Instagram Business account using the Instagram Graph API.

### Example Output

![Instagram Posting Result](ai%20safety%20insta.png)

## Future Enhancements

Future versions of this project will improve the workflow by:

- Separating captions, hashtags, and summaries into different Google Sheet columns
- Adding an approval step before posting
- Generating AI images automatically
- Improving error handling for expired access tokens
- Supporting multiple social media platforms

## Workflow Screenshot

![Workflow](Ai%20agent%20content%20creator.png)

## Features

- Reads YouTube URLs from Google Sheets
- Extracts video transcripts using Supadata API
- Generates Instagram captions using Groq AI
- Creates hashtags and content summaries
- Updates Google Sheets automatically
- Supports future Instagram auto-posting integration

## Project Status

Current Status: In Development

Completed:
- Google Sheets integration
- Transcript extraction
- AI caption generation
- Workflow automation in n8n

In Progress:
- Instagram Graph API integration
- Automated post publishing

## Requirements

Before using or enhancing this project, make sure the following tools and services are available:

Software Requirements
- n8n (Workflow Automation Platform)
- Google Account (for Google Sheets integration)
- Git and GitHub
- Modern web browser (Chrome, Edge, or Firefox)
  
API Requirements
- Groq API Key
- Supadata API Key
- Meta Developer Account
- Instagram Business or Creator Account
- Facebook Page connected to the Instagram account
- Instagram Graph API Access Token
- Google Sheets Setup

The Google Sheet should contain the following columns:

- Column
- videoUrl
- platform
- postTime
- status
- transcript
- caption
- approvalStatus
- hashtags
- imageUrl

## Recommended Workflow
1. Add a YouTube URL to Google Sheets.
2. Set the status to To Do.
3. Run the n8n workflow.
4. The workflow extracts the transcript.
5. AI generates captions, hashtags, and summaries.
6. Review the generated content.
7. Add or verify the image URL.
8. Approve the content.
9. Publish the post to Instagram.

## Technologies Used
- n8n
- Google Sheets
- Supadata API
- Groq AI
- Meta Graph API
- Instagram Graph API
- GitHub
