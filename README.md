# 🤖  LangChain Interview Practice Bot

> Part of my **90-Day LangChain + AI Job Search Journey**  
> Built by **Manpreet Kaur** | MS Data Science, Clarkson University | AI/ML Engineer

---

## 📌 What This Project Does

An AI-powered **Interview Practice Bot** that:
- Acts as a **technical interviewer for Data Science roles**
- Asks **one question at a time**
- Gives **feedback after each answer**
- **Remembers the full conversation** across multiple rounds using session-based memory

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| `LangChain` | Chain orchestration |
| `ChatGoogleGenerativeAI` | Gemini 2.5 Flash LLM |
| `ChatPromptTemplate` | System message + prompt formatting |
| `StrOutputParser` | Clean string output |
| `RunnableWithMessageHistory` | Conversation memory |
| `ChatMessageHistory` | Session-based history storage |
| `Google Colab` | Development environment |

---

## 🧠 Key Concepts Used

- **System Message** — gives the bot its interviewer personality and rules
- **MessagesPlaceholder** — inserts full conversation history into every prompt
- **Session ID** — keeps one interview conversation connected across all rounds
- **Memory** — bot remembers previous questions and answers in the same session

---

## 🔐 API Key Safety

This project uses **Colab Secrets** to store the API key safely.  
The actual key is **never written in the code or pushed to GitHub.**

```python
# Safe way — key stays in Colab Secrets
from google.colab import userdata
os.environ["GOOGLE_API_KEY"] = userdata.get("GEMINI_API_KEY")
```

To run this notebook:
1. Open in Google Colab
2. Go to 🔑 **Secrets** (left sidebar) → Add your `GEMINI_API_KEY`
3. Run all cells

---

## 📂 Project Structure

```
day5_langchain_interview_bot.ipynb   ← Main notebook
README.md                            ← This file
```

---

## 💬 Sample Interview Flow

```
YOU:          Hi, I am ready. Please start the interview.

INTERVIEWER:  Great! Let's begin. Can you explain the difference
              between supervised and unsupervised learning?

YOU:          Supervised learning uses labeled data...

INTERVIEWER:  Good answer! You correctly identified the key difference.
              Next question: What is overfitting and how do you handle it?
```

---

## 📅 90-Day Journey Progress

| Day | Topic | Status |
|---|---|---|
| Day 1 | LangChain Prompt Templates + LCEL pipe operator | ✅ Done |
| Day 2 | ChatOpenAI Deep Dive — temperature, SystemMessage | ✅ Done |
| Day 3 | Output Parsers + Memory + ChatMessageHistory | ✅ Done |
| Day 4 | Conversation Chain + RunnableWithMessageHistory | ✅ Done |
| Day 5 | Mini Project — Interview Practice Bot | ✅ Done |

---

## 👩‍💻 About Me

**Manpreet Kaur**  
MS Data Science — Clarkson University  
AI/ML Engineer — 3+ years experience at Wipro  
STEM OPT eligible till 2028  

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://linkedin.com)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black)](https://github.com)

---

*This project is part of a 90-day structured job search plan to land an AI/ML Engineer role.*
