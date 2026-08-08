# Workflow Guide

## Overview

The Smart Inbox Assistant processes incoming Gmail messages using n8n and an AI Agent.

## Workflow Process

1. Gmail Trigger receives a new email.
2. Edit Fields prepares the email data.
3. AI Agent analyzes the email.
4. Code Node processes the AI response.
5. IF Node checks the priority.
6. Gmail performs the appropriate action.
7. Google Sheets stores the processed information.

## Priority Routing

- High → Immediate email action
- Medium → Draft reply
- Low → Draft reply