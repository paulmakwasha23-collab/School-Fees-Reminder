# School-Fees-Reminder
Automated school fees reminders for Zimbabwe via Twilio + n8n

# Zumbani Fees Reminder 🇿🇼
Automated WhatsApp school fees reminders for Zimbabwe using n8n + Twilio.

## Problem
Private schools lose 30-60% revenue to late fees. Secretaries waste 40hrs/month calling parents. Kids get sent home with letters.

## Solution 
Google Sheets → n8n → Twilio WhatsApp API. Auto-texts parents 7 days before due date. Cost: $0.008/text. ROI: 4000% if 1 kid pays.

## Demo
[Screenshot of WhatsApp message]
> Zumbani Primary: Fees for Paul Makwasha $12 due 2026-04-28. EcoCash 0771234567

## Tech Stack
- n8n Cloud (free tier)
- Twilio Programmable Messaging 
- Google Sheets API
- WhatsApp Business API

## Results
Pilot: 5/5 parents received message. 3 paid within 48hrs. 0 kids sent home.

## Setup
1. See `/docs/setup-twilio.md` for API keys
2. Import `/n8n/workflow.json` to n8n
3. Copy `/sheets/template.csv` to Google Sheets
4. Add credentials to `.env` 

## Roadmap
- [x] Sandbox WhatsApp MVP
- [ ] WhatsApp Business API - May 2025
- [ ] Auto voice calls for defaulters
- [ ] EcoCash deep-link payments

## Disclaimer
Built for learning. Not affiliated with Zumbani Primary. Test with consent only.
