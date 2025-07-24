### Price Qualification Email Agent

Intelligent Client Filtering & Automated Gmail Responses Based on Price Agreement
Built with n8n, Google Forms, and Gmail API

## Overview
This workflow is designed to streamline client communications based on their price agreement status. It takes form submissions from potential customers, filters them by how closely they align with the requested price, and sends personalized follow-up emails accordingly.

Whether you’re negotiating service fees, selling products, or qualifying leads, this agent automates the process of identifying serious buyers and following up strategically—saving time and boosting conversion.

## Tools 

Form Submission: Collect client responses and price offers.
n8n: Automate filtering, email logic, and API communication.
Filter Node: Identifies clients matching asking price, close offers and low offers.
Gmail Node (Send Email): Delivers personalized follow-ups to qualified prospect clients.

## Workflow Summary

Client fills form → 
→ n8n retrieves response →
→ Filter by offer amount →
→ Email those matching asking price →
→ Email those close to price →
→ Optionally exclude or flag low offers

## ❌ Problem Statement

- Too many unqualified leads waste time  
- Manual filtering of client offers is repetitive and error-prone  
- Missed follow-up with high-intent clients reduces conversion  
- No efficient method to adapt email tone or content based on price alignment

## ✅ Solution Highlights

- 🎯 Automated Lead Qualification  
  Sorts clients into categories: ready to pay, close offers, and below threshold.

- 📤 Targeted Email Outreach  
  Sends polite decline, offer confirmation, or negotiation emails based on the client’s offer.

- ⚙️ Low-Code Setup  
  Built with n8n’s visual workflow editor—easy to customize without heavy coding.


## Example Use Case

- Asking Price: $500  
- Client A offers $500 → receives “Let’s begin!” confirmation email  
- Client B offers $470 → receives “We appreciate your interest, we’re close!” email  
- Client C offers $300 → no email sent (filtered out or flagged)

## How to Use

2️⃣ Import Workflow into n8n
- Upload the .json file to n8n  
- Configure Gmail credentials via OAuth  
- Link form data source (Google Sheets, webhook, or direct API)

3️⃣ Customize Parameters
- Set your asking price inside the Filter node  
- Adjust thresholds for “close to price” logic  
- Modify email content per group (use dynamic fields for personalization)

4️⃣ Deploy & Test
- Use a test form submission  
- Confirm filtering works correctly  
- Check Gmail inbox for outgoing messages

## Final Thoughts

This price-sensitive client responder helps turn form fills into deals. By qualifying clients intelligently and customizing outreach, it creates better engagement—and makes every lead count.
