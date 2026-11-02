# AI Monitoring & Incident Management System

### API Monitoring | Error Handling | No-Code Automation

An educational automation project built with **Make.com** to monitor API events, log technical failures, prevent duplicate records, and manage incident resolution.

## Project Overview

The system helps automate technical incident management by collecting events, validating incoming requests, tracking errors, and updating incident statuses.

## Key Features

- Secure webhook endpoint with API key authentication
- JSON request validation
- Duplicate event detection using Event ID
- Automatic event registration in Google Sheets
- Technical error logging
- Retry mechanisms for temporary API failures
- Incident lookup and resolution
- Structured HTTP responses

## Technologies

- Make.com
- Webhooks & HTTP API
- Google Sheets
- Make Data Store
- JSON
- API Key Authentication
- Router & Filters
- Error Handler

## Tested Results

| Test Case | Result |
|---|---|
| Valid new event | 200 LOGGED |
| Duplicate event | 200 ALREADY_LOGGED |
| Missing API key | 401 Unauthorized |
| Invalid request data | 400 REJECTED |
| Incident already resolved | 200 ALREADY_RESOLVED |
| Incident not found | 404 INCIDENT_NOT_FOUND |

## Architecture

The project consists of three main automation workflows:

1. **Secure Monitoring Center** — receives, validates, and logs API events.
2. **Automation Failure Logging** — records technical failures and supports recovery.
3. **Incident Resolution API** — searches for incidents, updates records, and manages resolution.

## Project Status

Completed educational prototype with successfully tested core functionality.

Additional security, concurrency, and reliability testing would be required before production deployment.

## Author

**Alan Sulaimanov**

Junior AI Automation Developer

GitHub: [ai-sulaimanovalan](https://github.com/ai-sulaimanovalan)

## Project Documentation

[View Project Portfolio (PDF)](./AI_Monitoring_Incident_Management_Portfolio_Final.pdf)

## Workflow Screenshots

### 1. Secure Monitoring Center
![Secure Monitoring Center](<./Центр мониторинга SECURE.png>)

### 2. Automation Failure Logging
![Automation Failure Logging](<./Журнал сбоев.png>)

### 3. Incident Resolution API
![Incident Resolution API](<./Закрытие инцидетов.png>)
