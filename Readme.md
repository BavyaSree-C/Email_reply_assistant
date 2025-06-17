
📧 Email Assistant AI
This project is an intelligent Gmail assistant that automatically:

✅ Fetches your latest emails from Gmail

✅ Classifies them into categories such as:

Personal

Job Offer

Job Application Updates

(and others like Newsletter, Finance, Promotion, etc.)

✅ Generates smart, context-aware replies for the first 3 categories

✅ Saves those replies as drafts in your Gmail

🚀 Demo Features
Feature	Description
🔐 Gmail OAuth2 Authentication	Uses credentials.json and token.json for access
✨ OpenRouter AI Classification	Classifies email based on subject and snippet
🤖 GPT-Powered Reply Generation	Generates polite and relevant replies
💾 Gmail Draft Creation	Replies are saved as drafts, not sent automatically

📦 Setup Instructions
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/BavyaSree-C/Email_reply_assistant.git
cd email-assistant-ai
2. Install Requirements
bash
Copy
Edit
pip install -r requirements.txt
3. Set Up Gmail API
Go to Google Cloud Console

Create a new project

Enable the Gmail API

Download credentials.json and place it in your project directory

4. Create .env File
env
Copy
Edit
OPENROUTER_API_KEY=your_openrouter_api_key_here
Get your API key from https://openrouter.ai

5. Run the Assistant
python email_assistant.py

🧠 Email Categories
Only these categories will trigger automated replies:

Personal – e.g., casual conversations

Job Offer – e.g., interview invites or offer letters

Job Application Updates – e.g., updates on your application status

Other types (e.g., newsletters, finance, promotions) are skipped.

📂 Output
Replies are saved as drafts in your Gmail

You can review and manually send them

🔐 Security Notice
Make sure to add the following files to .gitignore:

gitignore
Copy
Edit
.env
token.json
credentials.json
🛠 Tech Stack
Python

OpenRouter (LLM via GPT-3.5 / GPT-4)

Google Gmail API

LangChain (Gmail utils)

💡 Future Improvements
 Auto-send with confirmation

 Summarize full threads

 Web UI with Streamlit

📜 License
MIT License

