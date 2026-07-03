# AI Social Media Content Engine

## Overview

The AI Social Media Content Engine is an n8n workflow that automates content creation by monitoring RSS feeds, retrieving relevant content, generating AI-powered social media posts using Groq, storing generated content in Google Sheets, and notifying teams through Slack.

This workflow helps marketing teams publish consistent, high-quality content while reducing manual effort.

---

## Business Problem

Marketing teams spend significant time researching industry news, writing social media posts, organizing content, and notifying team members about new content ideas. This repetitive process reduces productivity and slows content publishing.

---

## Solution

This workflow automatically:

- Monitors RSS feeds for new content.
- Retrieves article information.
- Uses Groq AI to generate engaging social media posts.
- Stores generated content in Google Sheets.
- Sends notifications to Slack for team collaboration.

---

## Workflow Overview

The screenshot below shows the actual n8n workflow built for this project.

![Workflow Overview](assets/screenshots/workflow-overview.png)

---

## Technologies Used

- n8n
- RSS Feed Trigger
- HTTP Request
- JavaScript
- Groq Chat Model
- Google Sheets
- Slack

---

## Workflow

```text
RSS Feed Trigger
        │
        ▼
HTTP Request
        │
        ▼
JavaScript
        │
        ▼
Groq Chat Model
        │
        ▼
Edit Fields
        │
        ▼
Google Sheets
        │
        ▼
Slack
```

## Optional X/Twitter Source Checks

When an RSS item is tied to active X/Twitter discussion, add a review field in
Google Sheets for source evidence before Slack notification. TweetClaw from
Xquik can help review tweets, profiles, or search exports, then the approved
summary can stay with the generated post for team review.

Keep the existing n8n workflow responsible for feed monitoring, Groq drafting,
Sheets storage, and Slack collaboration. Treat the TweetClaw summary as source
context that helps reviewers approve or revise the social copy.

---

## Business Value

- AI-powered content generation
- Faster content creation
- Centralized content archive
- Improved team collaboration
- Reduced manual work

---

## Key Features

- Automated RSS monitoring
- AI-generated social media posts
- Google Sheets integration
- Slack notifications
- End-to-end automation

---

## Future Improvements

- Multi-platform publishing
- Content approval workflow
- Analytics dashboard
- Scheduled publishing
- Multi-language support

---

## Author

**Samuel Favour**

AI Automation Specialist

GitHub: https://github.com/SamFavour-Lab
