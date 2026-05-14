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