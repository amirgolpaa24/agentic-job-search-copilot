# Workflow Notes

## 1. Manual Job Tracker

### Purpose
Manually enter a job lead in n8n and append it to the Google Sheets job tracker.

### Nodes
1. Manual Trigger
2. Set Job Input
3. Prepare Job Row
4. Google Sheets - Append Row

### Output
A new row is added to the `Jobs` tab in the Google Sheet.

### What this proves
- Local n8n is running through Docker
- Google Sheets OAuth credentials work
- n8n can transform data using a Code node
- n8n can save structured job data to the tracker

## 2. Webhook Job Intake

### Purpose
Receive job information through a POST request and append it to the Google Sheets tracker.

### Nodes
1. Webhook Trigger
2. Prepare Job Row
3. Google Sheets - Append Row

### What this proves
- n8n can expose an HTTP endpoint
- External systems can send job data into the workflow
- The workflow can normalize and save structured job records