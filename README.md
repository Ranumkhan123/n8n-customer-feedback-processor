# The Intelligent Customer Feedback Processor

This n8n workflow automatically collects customer feedback through a form, processes it using an LLM (AI model), and classifies it into **Positive, Negative, or Neutral** categories for smarter insights.

---

##  Features
- Collects customer feedback via an n8n form  
- Uses an **LLM (Large Language Model)** for intelligent feedback classification  
- Routes feedback into **Positive, Negative, and Neutral** categories  
- Easy to extend for CRM, Google Sheets, or Email notifications  

---

## How It Works
1. **Form Node** → Collects Name, Email, and Feedback from users  
2. **LLM Node** → Analyzes and classifies the feedback text  
3. **Routing Logic** → Directs feedback into separate flows:
    - **Positive Feedback** 
     - Sends a **thank you response** to the user.  
     - Optionally logs feedback for testimonials or future marketing use.  
   - **Neutral Feedback** 
     - Sends a **polite acknowledgment** message.  
     - Routes feedback to an **internal review queue** for further evaluation.  
   - **Negative Feedback** 
     - Sends an **apology email** to the customer.  
     - Creates a **ticket in the support system** for the team to follow up.  
4. **Output** → Displays a thank-you message after submission  

---

## Demo
View the live demo → [Video overview](docs/demo.md)

---

##  Setup
1. Import the workflow JSON file into your **n8n instance**  
2. Configure the **LLM node** with your preferred provider (OpenAI / Ollama / etc.)  
3. Run the workflow and share the form link with users  

---

## Repository Contents
- `workflow.json` → The exported n8n workflow file  
- `README.md` → Documentation  

---

## Contributing
Feel free to fork this repository and enhance the workflow with:  
- Additional LLM prompts for deeper sentiment analysis  
- Integration with CRMs (e.g., HubSpot, Salesforce)  
- Slack / WhatsApp alerts for negative feedback  

---
##  Author

**Ranum Khan**  
[LinkedIn](https://linkedin.com/in/ranum-khan-qaengineer) | [GitHub](https://github.com/Ranumkhan123)  
Experienced **QA Engineer** with a strong foundation in manual and API testing, and rich documentation.

---


## License
This project uses public APIs and is intended for educational and portfolio purposes only.
