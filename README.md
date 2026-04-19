#  HealthBot — AI-Powered Health Assistant (Groq + LLaMA 3)

HealthBot is a lightweight AI-powered health assistant built with Python and Groq’s LLaMA 3 API.  
It provides general health information, symptom awareness guidance, and wellness tips in a safe, conversational format.

> ⚠️ This project is for educational purposes only and does NOT provide medical diagnosis or treatment.

---

##  Key Features

- 🤖 AI-powered conversational health assistant
- ⚡ Fast inference using Groq API (LLaMA 3 models)
- 🛡️ Built-in safety filter for harmful or emergency queries
- 🧠 Conversation memory for contextual responses
- 💬 Interactive chat mode (Colab / terminal)
- 🔒 Secure API key handling (no hardcoding)

---

##  AI Model

- **Model Used:** `llama3-8b-8192` (via Groq API)
- Optimized for fast, conversational responses

---

##  Installation

Clone the repository:

```bash
git clone https://github.com/your-username/healthbot.git
cd healthbot

Install dependencies:

pip install groq python-dotenv
## API Key Setup

HealthBot requires a Groq API key.

1. Get API Key

Create your free API key here:
 https://console.groq.com

2. Set Environment Variable
💻 Linux / Mac
export GROQ_API_KEY="your_api_key_here"
🪟 Windows (CMD)
set GROQ_API_KEY=your_api_key_here
☁️ Google Colab
import os
os.environ["GROQ_API_KEY"] = "your_api_key_here"
 Running the Project
python healthbot.py

Or in Google Colab:

Run all cells
Start chat using run_chat()
💬 Example Usage
User: I have a sore throat and mild fever.

HealthBot:
It may be caused by a viral infection or irritation. Drink warm fluids, rest, and stay hydrated...
Please consult a qualified healthcare professional for personalised advice.
🛡️ Safety System

HealthBot includes a multi-layer safety system:

🚫 Blocked Queries
Self-harm or suicide-related content
Drug overdose or illegal drug instructions
Harmful or dangerous medical instructions
⚠️ Emergency Detection

Automatically detects symptoms like:

Chest pain
Difficulty breathing
Stroke-like symptoms

and advises immediate medical attention.

## Project Structure
healthbot/
│
├── healthbot.py        # Main chatbot code
├── README.md           # Project documentation
├── .gitignore          # Ignore sensitive files
🔒 Security Best Practices
❌ API keys are NOT hardcoded
✅ Uses environment variables
✅ Supports .env file setup
❌ No sensitive data stored in repo
⚠️ Disclaimer

HealthBot is NOT a medical professional.
It provides general informational responses only and must NOT be used for diagnosis or treatment.

Always consult a qualified healthcare provider for medical concerns.

## Author
Yahya Abbasi
Developed using:

Python 
Groq API 
Meta LLaMA 3 
## Future Improvements
 Web UI (Streamlit / Flask)
 Mobile-friendly interface
 Medical knowledge base integration
 Advanced memory system
