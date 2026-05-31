# 🤖 LangChain Interview Practice Bot

Built by **Manpreet Kaur** | MS Data Science, Clarkson University | AI/ML Engineer

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

## 👩‍💻 About Me

**Manpreet Kaur**
MS Data Science — Clarkson University
AI/ML Engineer — 3+ years experience at Wipro
STEM OPT eligible till 2028

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://linkedin.com)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black)](https://github.com)
