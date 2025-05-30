 Chainlit Setup Guide for Panaversity AI Assistant
This guide walks you through setting up and running the Chainlit-based AI assistant that uses the Gemini API. Developed by Farhad Ali Laghari, this chatbot responds in English, Urdu, and Sindhi, and introduces its creator when asked.

📦 Prerequisites
Python 3.10 or higher

pip

Gemini API key from Google AI Studio

Git (optional but recommended)

Virtual environment support

⚙️ Installation Steps
Clone the Project

bash
Copy
Edit
git clone https://github.com/your-username/panaversity-ai-assistant.git
cd panaversity-ai-assistant
Set Up a Virtual Environment

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
Install Required Libraries

bash
Copy
Edit
pip install -r requirements.txt
Add Your Gemini API Key

Create a .env file in the root of your project:

ini
Copy
Edit
GEMINI_API_KEY=your_google_gemini_api_key_here
🚀 Run Chainlit App
Start the Chainlit app using:

bash
Copy
Edit
chainlit run app.py
Chainlit will open your chatbot in the browser (usually at http://localhost:8000).

🧠 Chatbot Behavior
Responds based on Google Gemini 2.0 Flash

Automatically replies in the same language as the user: English, Urdu, or Sindhi

Provides a custom introduction for the creator when asked:

"Who created you?"

"Who is your developer?"

"Who made you?"

🧪 Testing It
Try these in the chat:

Who created you?

توهان ڪير آهيو؟

آپ کہاں سے ہیں؟

🧼 Resetting or Restarting
To reset the environment:

bash
Copy
Edit
deactivate
rm -rf venv
To re-run the app, re-activate the virtual environment and run Chainlit again.

📁 File Structure Overview
bash
Copy
Edit






panaversity-ai-assistant/
│
├── app.py               # Main Chainlit application
├── agents/              # Custom agent and config setup
├── .env                 # Your Gemini API key
├── requirements.txt     # Python dependencies
├── README.md            # Project overview
└── chainlit.md          # Chainlit-specific guide (this file)



