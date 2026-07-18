This project automates the process of finding local business leads, verifying contact information, generating personalized outreach emails, and sending them via Brevo. It removes the need for manual data entry and ensures high-quality lead targeting.

🛠️ Technology Stack
Automation Platform: Make (formerly Integromat)

Lead Enrichment: Hunter.io API

Content Generation: Google Gemini AI

Email Sending: Brevo

⚙️ How It Works
Webhook Trigger: Receives raw business data (Business Name, City, etc.) from a terminal script.

Hunter.io API: Performs a domain-search to identify valid professional email addresses associated with the business.

Filter/Gatekeeper: Automatically discards leads without valid contact information to save API credits.

Gemini AI: Generates a hyper-personalized email based on the business category and location.

Brevo: Sends the finalized email to the identified contact.

📋 Setup Instructions
API Keys: Ensure your Hunter.io and Brevo API keys are active within your Make modules.

Webhook: Update your terminal scraper script to point to the endpoint provided by the Webhook module.

Mapping: Ensure the output from Hunter (emails[].value) is correctly mapped to the Brevo "To" field.

AI Integration: Link the Gemini Result pill directly into the Brevo "Text Body" field to ensure the full AI-generated message is sent.
