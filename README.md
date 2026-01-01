# AI-Driven Form Intelligence Enrichment Pipeline (n8n)

An n8n workflow that enriches Google Form submissions using public inference APIs and an LLM, then sends a personalized email response.

---

## What This Workflow Does

- Triggers on Google Form submission  
- Generates a sequential internal ID  
- Stores raw submission data in Google Sheets  
- Enriches data using:
  - Genderize (gender prediction)
  - Nationalize (nationality inference)
  - Agify (age estimation)
- Updates the sheet with enriched attributes  
- Uses OpenAI to generate a response message  
- Sends the response via Gmail  

---

## Tech Stack

- n8n  
- Google Forms & Google Sheets  
- OpenAI API  
- Public inference APIs (Genderize, Nationalize, Agify)  
- Gmail API  

---

## How to Use

1. Import `workflows/form-intelligence-enrichment.json` into n8n  
2. Configure credentials inside n8n:
   - Google Sheets  
   - Gmail  
   - OpenAI  
3. Update Sheet IDs and field mappings  
4. Activate the workflow  

---

## Notes

- No credentials are stored in this repository  
- Designed for internal automation and learning purposes  

---

## License

MIT
