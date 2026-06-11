# Project Overview – AI Content Summarizer

## Introduction

AI Content Summarizer is a workflow automation project developed using n8n, Google Sheets, and Google's Gemini API. The system automates the process of generating concise summaries from textual content stored in spreadsheets. By integrating Artificial Intelligence with workflow automation, the project eliminates repetitive manual summarization tasks and improves productivity.

The project demonstrates practical implementation of API integration, workflow orchestration, OAuth2 authentication, JSON data processing, and AI-powered automation.

---

## Problem Statement

Organizations and individuals often manage large amounts of textual information such as reports, articles, notes, and documentation. Manually summarizing such content requires significant time and effort.

The objective of this project is to automate the summarization process by:

* Reading content from Google Sheets.
* Sending the content to an AI model.
* Generating concise summaries automatically.
* Updating the generated summaries back into the spreadsheet.

---

## Project Objectives

* Automate content summarization using Artificial Intelligence.
* Integrate Google Sheets with external AI services.
* Implement secure API communication using OAuth2.
* Build a scalable low-code workflow using n8n.
* Reduce manual effort in content processing tasks.

---

## System Architecture

The workflow consists of five major components:

1. Google Sheets Data Source
2. n8n Workflow Engine
3. Gemini API Integration
4. Summary Extraction Logic
5. Google Sheets Update Module

Workflow Execution:

Google Sheets → Fetch Content → Gemini API → Extract Summary → Update Google Sheets

---

## Workflow Design

### Step 1: Read Content from Google Sheets

The workflow retrieves records from a Google Sheet containing:

* ID
* Content
* Summary

The content field serves as the input for AI processing.

### Step 2: Send Request to Gemini API

The content is forwarded to Google's Gemini API using an HTTP Request node.

The API receives a prompt requesting a concise summary of the provided text.

### Step 3: Process AI Response

Gemini generates a summarized version of the content and returns the result in JSON format.

The workflow extracts the summary from the API response using expression-based data mapping.

### Step 4: Update Spreadsheet

The generated summary is written back into the corresponding row of Google Sheets.

This creates a complete end-to-end automation pipeline.

---

## Technologies Used

### Workflow Automation

* n8n

### Artificial Intelligence

* Google Gemini API

### Data Storage

* Google Sheets

### Authentication

* OAuth2

### Integration

* REST API
* JSON

### Cloud Services

* Google Cloud Platform

---

## Key Features

* Automated content summarization.
* Multi-row spreadsheet processing.
* AI-powered text analysis.
* Dynamic row-level updates.
* Secure OAuth2 authentication.
* Low-code workflow implementation.
* Scalable automation architecture.

---

## Challenges Faced

During development, several technical challenges were encountered:

### API Authentication

Configuring OAuth2 credentials and integrating Google services securely within n8n.

### Workflow Data Mapping

Ensuring data flowed correctly between workflow nodes while maintaining row-level context.

### Multi-Row Processing

Handling multiple spreadsheet records and updating the correct rows with generated summaries.

### API Response Parsing

Extracting summary text from nested JSON responses returned by the Gemini API.

---

## Results

The workflow successfully:

* Reads content automatically from Google Sheets.
* Generates AI-powered summaries using Gemini.
* Updates corresponding spreadsheet rows automatically.
* Processes multiple records within a single workflow execution.

The project demonstrates a practical application of Artificial Intelligence and workflow automation for business productivity.

---

## Learning Outcomes

Through this project, the following concepts were implemented and practiced:

* Workflow Automation
* API Integration
* OAuth2 Authentication
* REST API Communication
* JSON Data Processing
* Google Cloud Services
* Spreadsheet Automation
* AI Application Development
* Low-Code Development Platforms

---

## Future Enhancements

Potential improvements include:

* Real-time execution using Google Sheets triggers.
* Multi-language summarization support.
* Sentiment analysis integration.
* Email notifications for processed records.
* Web dashboard for workflow monitoring.
* Cloud deployment using Docker and VPS infrastructure.
* Integration with additional AI models.

---

## Conclusion

The AI Content Summarizer project successfully combines workflow automation and Artificial Intelligence to automate content summarization tasks. The project provides hands-on experience with modern automation tools, cloud services, API integration, and AI technologies while demonstrating a practical real-world use case for business process automation.

---

Author: Subham Raj
