# AI-Driven Form Intelligence Enrichment Pipeline (n8n)

This project contains an **n8n workflow** that enriches Google Form submissions using public inference APIs and LLMs, then sends a personalized email.

## What This Workflow Does

1. Triggers on Google Form submission  
2. Generates a sequential internal ID  
3. Stores raw submission in Google Sheets  
4. Enriches data using:
   - Genderize (gender prediction)
   - Nationalize (nationality inference)
   - Agify (age estimation)
5. Updates the sheet with enriched attributes  
6. Uses OpenAI to generate a response message  
7. Sends the response via Gmail

## Tech Stack

- n8n
- Google Forms & Google Sheets
- OpenAI API
- Public inference APIs (Genderize, Nationalize, Agify)
- Gmail API

## How to Use

1. Import `workflows/form-intelligence-enrichment.json` into n8n
2. Configure credentials inside n8n:
   - Google Sheets
   - Gmail
   - OpenAI
3. Update Sheet IDs and field mappings
4. Activate the workflow

## Notes

- No credentials are stored in this repository
- This workflow is designed for educational and internal automation use

## License

MIT
