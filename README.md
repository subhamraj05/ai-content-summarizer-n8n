# AI Content Summarizer using n8n & Gemini API

## Overview

AI Content Summarizer is a workflow automation project built using n8n, Google Sheets, and Google's Gemini API. The system automatically reads content from a Google Sheet, generates AI-powered summaries, and updates the generated summaries back into the corresponding spreadsheet rows.

The project demonstrates practical implementation of workflow automation, API integration, OAuth2 authentication, data processing, and AI-powered business automation.

---

## Features

* Automated content summarization using Google's Gemini API.
* Google Sheets integration for data storage and processing.
* Multi-row content processing workflow.
* Automated spreadsheet updates with generated summaries.
* OAuth2-based secure authentication.
* REST API integration and JSON data handling.
* Low-code workflow automation using n8n.

---

## Workflow Architecture

```text
Google Sheets
      ↓
Read Content Rows
      ↓
Gemini API
      ↓
Generate Summary
      ↓
Extract Response
      ↓
Update Google Sheets
```

---

## Technologies Used

* n8n
* Google Gemini API
* Google Sheets API
* Google Drive API
* OAuth2 Authentication
* REST APIs
* JSON Data Processing

---

## Project Workflow

1. Fetch content records from Google Sheets.
2. Send content to Gemini API through HTTP requests.
3. Generate AI-powered summaries.
4. Extract summary text from the API response.
5. Update the corresponding spreadsheet row automatically.
6. Store generated summaries for future reference.

---

## Screenshots

### Workflow Design

<img src="screenshots/workflow.png" alt="Workflow" width="100%">

### Input Data

<img src="screenshots/google-sheet-input.png" alt="Input Sheet" width="100%">

### Generated Summaries

<img src="screenshots/google-sheet-output.png" alt="Output Sheet" width="100%">

---

## Learning Outcomes

This project helped in gaining hands-on experience with:

* Workflow Automation
* API Integration
* OAuth2 Authentication
* Google Cloud Services
* JSON Parsing and Data Mapping
* Spreadsheet Automation
* AI Application Development
* Low-Code Development Platforms

---

## Future Enhancements

* Automatic trigger-based execution when new rows are added.
* Batch content processing.
* Multi-language summarization support.
* Email notification integration.
* Web dashboard for workflow monitoring.
* Cloud deployment using VPS or Docker.

---

## Repository Structure

```text
ai-content-summarizer-n8n/
│
├── README.md
├── workflow/
│   └── AI Content Summarizer Workflow.json
│
├── docs/
│   └── project-overview.md
│
└── screenshots/
    ├── workflow.png
    ├── google-sheet-input.png
    └── google-sheet-output.png
```

---

## Author

**Subham Raj**

B.Tech in Computer Science Engineering

GitHub: https://github.com/subhamraj05
