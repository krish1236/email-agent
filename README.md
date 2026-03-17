# Email Digest Agent

A simple agent that reads your recent emails, creates a summary digest, and sends it to you. Built on Runforge.

## What it does

1. **Reads inbox** (safe step) — Fetches your recent emails via connected Gmail
2. **Creates digest** (safe step) — Summarizes emails into a readable format
3. **Sends digest** (commit step) — Sends the summary email, requires your approval first

## Tools required

- Gmail (read + send)

## Usage

Deploy on Runforge:
1. Create a new project → connect this repo
2. Enable managed tools → add Gmail
3. Connect your Gmail account
4. Trigger a run

## Input (optional)

```json
{
  "recipient": "you@example.com",
  "max_emails": 5
}
```

If no recipient is specified, the digest is sent to your own inbox.
