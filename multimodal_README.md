# ✈️ FlightAI — Airline Assistant with Tool Calling

FlightAI is an intelligent airline assistant powered by OpenAI that provides fast, accurate ticket pricing through a structured tool-calling workflow. It combines an LLM with a SQLite database and a clean Gradio interface to demonstrate how real-world AI assistants can interact with external systems safely and reliably.

Built for learning, experimentation, and as a strong portfolio project demonstrating:

- Tool/function calling  
- Database integration  
- LLM orchestration  
- Environment-based secret management  
- Interactive UI with Gradio  

---

## 🚀 Features

✅ Natural language airline assistant  
✅ Real-time ticket lookup from a SQLite database  
✅ Function/tool calling architecture  
✅ Clean and minimal UI using Gradio  
✅ Secure API key handling via `.env`  
✅ Lightweight and easy to run locally  

---

## 🧠 How It Works

1. The user asks for a ticket price.
2. The model determines it needs structured data.
3. A tool (`get_ticket_price`) is called.
4. The assistant responds with a concise, accurate answer.

This mirrors how production AI agents interact with backend services.

---

## 📦 Project Structure

```
project7.ipynb   → Main notebook with assistant logic
prices.db        → SQLite database storing ticket prices
.env             → API keys (DO NOT COMMIT)
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone <your-repo-url>
cd <repo-name>
```

---

### 2. Install Dependencies

```bash
pip install openai python-dotenv pillow gradio
```

(You may optionally create a virtual environment.)

---

### 3. Add Your OpenAI API Key

Create a `.env` file:

```
OPENAI_API_KEY=your_api_key_here
```

⚠️ **Never upload `.env` to GitHub.**

---

### 4. Run the Notebook

Launch:

```bash
jupyter notebook
```

Open `project7.ipynb` and run all cells to start the assistant locally.

---

## 🧪 How Others Can Use This Project

This project is ideal for:

- Learning tool/function calling
- Understanding LLM + database workflows
- Building production-style AI assistants
- Experimenting with Gradio interfaces
- Extending into multi-tool agents

### Ideas for Extension

- Add more destinations dynamically  
- Connect to a real flight API  
- Implement booking capability  
- Add user authentication  
- Deploy as a web app  
- Upgrade to a multi-agent architecture  

---

## 🔐 Security Notes

✔ No API keys are stored in the code  
✔ Uses environment variables  
✔ Safe for public repositories (when `.env` is ignored)

If a key is ever exposed, rotate it immediately from your OpenAI dashboard.

---

## 💡 Why This Project Matters

Modern AI systems don’t just chat — they take actions.

FlightAI demonstrates the transition from passive LLMs to agentic systems that interact with real data sources — a critical pattern in next-generation software.

---

## ⭐ Support

If you found this project useful, consider giving the repository a star!
