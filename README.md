Thanks for the updated code!

Based on your latest script, **Tavily is *not* used** — you're using a **custom `SafeDuckDuckGoSearchRun`**, along with **Wikipedia** and **Arxiv** as tools, inside a LangChain agent powered by **Groq LLaMA3-70B**.

Here’s your updated, corrected, and clean `README.md` — **focused on DuckDuckGo**, **not Tavily**:

---

````markdown
# 🔍 Web Search Chatbot using LangChain, Groq, DuckDuckGo, Wikipedia & Arxiv

This project is a **real-time web search chatbot** built with [LangChain](https://www.langchain.com/), [Groq](https://groq.com), and a set of research & web tools including:

- 🦆 **DuckDuckGo** (for general web search)
- 📚 **Arxiv** (for academic papers)
- 🧠 **Wikipedia** (for encyclopedic knowledge)

The app allows you to ask **any kind of question**, and the chatbot will search across the web and answer using **Groq’s blazing-fast LLaMA3-70B model**.

---

## 🧠 How It Works

1. User asks a question via chat.
2. The app uses LangChain to initialize an **agent**.
3. The agent is equipped with 3 tools:
   - DuckDuckGo (with custom rate-limit-safe wrapper)
   - Arxiv search
   - Wikipedia lookup
4. Groq LLM processes the inputs and generates a response.
5. Results are streamed directly into the Streamlit chat UI.

---

## 📁 Project Structure

```bash
.
├── app.py              # Main Streamlit app
├── .env                # Environment variables (GROQ_API_KEY)
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
````

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/web-search-chatbot.git
cd web-search-chatbot
```

### 2️⃣ Create a Virtual Environment

```bash
uv venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3️⃣ Install Dependencies

```bash
uv pip install -r requirements.txt
# or
pip install -r requirements.txt
```

### 4️⃣ Create `.env` file

```env
GROQ_API_KEY=your_groq_api_key
```

---

## 🚀 Run the App

```bash
streamlit run app.py
```

Open in browser at: [http://localhost:8501](http://localhost:8501)

---

## 💡 Example Prompts

* “What is LangChain?”
* “Find the latest Arxiv paper on Transformer models.”
* “Who invented self-attention?”
* “Summarize quantum computing from Wikipedia.”

---

## 🛠️ Tech Stack

* 🧠 **LangChain Agents**
* 🤖 **Groq LLM (LLaMA3-70B)**
* 🔍 **DuckDuckGo Web Search**
* 📚 **Arxiv API**
* 📖 **Wikipedia API**
* 🧵 **Streamlit Chat UI**

---

## 📦 requirements.txt

```
streamlit
python-dotenv

langchain
langchain-core
langchain-community
langchain-groq
langchain-openai
langchain-text-splitters

duckduckgo-search
arxiv
wikipedia
```

---

## 🎓 About Me

I'm currently an **MCA final-year student**, experimenting with **agentic LLM tools**, real-time APIs, and conversational AI.

🔍 This project demonstrates how modern LLMs like Groq’s LLaMA3 can interact with multiple tools using LangChain's agent framework.

📌 Actively looking for roles in:

* 🧠 LLM + RAG Systems
* 🤖 Agentic AI
* ⚙️ MLOps / AI Tooling
* 📊 Applied Data Science

🔗 [LinkedIn](https://www.linkedin.com/in/yourname)
🌐 [Portfolio](https://yourwebsite.com)

---

## 🔧 Future Improvements

* Add Tavily or SerpAPI for robust search fallback
* Add memory and reranking
* Export chat history to markdown or PDF
* Deploy to Hugging Face Spaces or Streamlit Cloud

---

⭐ **If you found this useful, give it a star and feel free to fork!**

```

---

Let me know:
- If you want the **dark theme banner** for this project as well
- If you plan to eventually **switch from DuckDuckGo to Tavily**, so I can prepare that README version too

Ready for the next project whenever you are!
```
