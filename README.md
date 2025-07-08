🔗 👉 **[Watch the Demo on YouTube](https://www.youtube.com/watch?v=rg7M0oZdpFM&list=PLe-YIIlt-fbO3hXVoaPK56ikWRT0A9Gzr&index=4&ab_channel=Jatin)**
# 🔍 Web Search Chatbot using LangChain, Groq, DuckDuckGo, Wikipedia & Arxiv

This project is a **real-time web search chatbot** built with [LangChain](https://www.langchain.com/), [Groq](https://groq.com), and a set of intelligent research tools including:

- 🦆 **DuckDuckGo** (for general web search)
- 📚 **Arxiv** (for academic papers)
- 🧠 **Wikipedia** (for encyclopedic knowledge)

It uses LangChain’s agent framework and Groq’s blazing-fast **LLaMA3-70B** model to answer any question — with smart tool use and natural conversations, all in a clean Streamlit UI.

---

## 🧠 How It Works

1. Ask a question in the chat.
2. A LangChain **Agent** is initialized with access to:
   - 🔍 DuckDuckGo (via custom safe wrapper)
   - 📖 Wikipedia search
   - 📚 Arxiv API
3. The question is routed through tools as needed.
4. **Groq LLaMA3-70B** processes and returns the best possible answer.
5. The full chain + answer is streamed in the chat window using **Streamlit**.

---

## 📁 Project Structure

```bash
.
├── app.py              # Streamlit app code
├── .env                # Stores your Groq API key
├── requirements.txt    # Python dependencies
└── README.md           # You're reading it!
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/jatinydav557/real-time-search-engine-langchain.git
cd real-time-search-engine-langchain
```

### 2️⃣ Create a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
```

### 3️⃣ Install Dependencies

```bash
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

Then open: [http://localhost:8501](http://localhost:8501)

---

## 💬 Example Prompts

- “What is LangChain used for?”
- “Find a recent Arxiv paper on diffusion models.”
- “Who invented the attention mechanism?”
- “Give me a short summary of Generative AI from Wikipedia.”

---

## 🛠️ Tech Stack

| Tool / Lib         | Role                                     |
|--------------------|------------------------------------------|
| 🧠 LangChain        | Agent framework + tool routing           |
| 🤖 Groq LLaMA3-70B  | High-speed LLM                           |
| 🦆 DuckDuckGo       | General web search results               |
| 📚 Arxiv API        | Academic paper lookup                    |
| 📖 Wikipedia        | Encyclopedic knowledge tool             |
| 🎨 Streamlit        | Chat interface and UI                   |

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

## 🙋‍♂️ About Me

Hey, I’m **Jatin** — a final-year **MCA student**, passionate about building GenAI tools using **LLMs, LangChain, RAG pipelines, and conversational AI**.

📌 I’m currently building over **20+ projects** as part of my AI portfolio to land a top-tier role in:

- 🤖 LLM / GenAI Engineering  
- 📊 Applied Data Science  
- 🧠 NLP + Retrieval-Augmented Generation  
- ⚙️ MLOps & Tooling

---

## 🤝 Let's Connect

- **💼 LinkedIn:** [linkedin.com/in/jatin557](https://www.linkedin.com/in/jatin557)  
- **📦 GitHub:** [github.com/jatinydav557](https://github.com/jatinydav557)  
- **📬 Email:** [jatinydav557@gmail.com](mailto:jatinydav557@gmail.com)  
- **📱 Contact:** [+91-7340386035](tel:+917340386035)  
- **🎥 YouTube:** [See My Other AI Projects](https://www.youtube.com/@jatinML/playlists)

---

## 🧭 What’s Next?

- [ ] Add SerpAPI or Tavily for fallback search
- [ ] Add memory for chat history continuity
- [ ] Deploy to Hugging Face / GCP / Streamlit Cloud
- [ ] Add PDF export or markdown export for Q&A logs

---

⭐ If you liked this project, **star it**, fork it, or share it — it really helps!

> “Build tools that help others *think better* — that’s where AI shines.”
