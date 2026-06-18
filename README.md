# 🤖 TerminalMind

**TerminalMind** is an AI-powered Linux Copilot Agent that enables users to interact with their Linux system using natural language. Built with Python, Mistral LLM, SQLite, and Streamlit, it combines conversational AI with system-level tooling.

---

## 📌 Project Overview

TerminalMind bridges the gap between human language and Linux command-line operations. Instead of remembering commands or interpreting complex terminal outputs, users can simply ask questions in plain English.

Example:

```
User:
Create a file called notes.txt

TerminalMind:
✅ File "notes.txt" created successfully.
```

---

## ✨ Features

- 🧠 Persistent conversation memory
- 👤 Long-term user profile storage
- 💻 System monitoring
  - CPU Usage
  - RAM Usage
  - Available Memory
- 📂 File and folder management
- 📍 Current directory lookup
- 🐍 Python file discovery
- 🕒 Date and time retrieval
- 📝 Conversation logging
- 📊 Streamlit statistics dashboard
- 🤖 Local Mistral LLM integration
- 💾 SQLite-backed memory

---

## 🏗️ Architecture

```

┌─────────────────────┐
│ Streamlit Frontend  │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│    Agent Router     │
└──────────┬──────────┘
│
├──────────────┐
│              │
▼              ▼
LLM         Python Tools
(Mistral)   (CPU, Files, Time)

│
▼

SQLite Memory

```

---

## 📂 Project Structure

```

TerminalMind/
│
├── app.py
├── terminalmind.py
├── README.md
│
├── core/
│   └── agent.py
│
├── memory/
│   ├── chat_memory.py
│   └── database.py
│
├── profile/
│   └── user_profile.py
│
├── tools/
│   ├── system_tool.py
│   ├── os_tool.py
│   ├── time_tool.py
│   ├── file_tool.py
│   ├── logger_tool.py
│   └── stats_tool.py
│
├── screenshots/
│
└── docs/

```

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|----------|
| Python | Core Development |
| Ollama | Local LLM Runtime |
| Mistral | Language Model |
| Streamlit | Frontend UI |
| SQLite | Persistent Storage |
| SQLAlchemy | ORM |
| Git | Version Control |
| GitHub | Repository Hosting |

---

## 🚀 Installation

### Clone the repository

```bash
git clone https://github.com/Gilliloves/TerminalMind.git

cd TerminalMind
```

### Create virtual environment

**Windows**

```bash
python -m venv venv

venv\Scripts\activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run Ollama

```bash
ollama serve
ollama run mistral
```

### Launch the application

```bash
streamlit run app.py
```

---

## 📸 Screenshots

### Main Interface

![Main Interface](screenshots/main_interface.png)

### Memory System

![Memory System](screenshots/memory_system.png)

### File Creation

![File Creation](screenshots/file_creation.png)
---

## 🔮 Future Enhancements

- PDF document understanding
- Retrieval-Augmented Generation (RAG)
- Voice interaction
- Docker monitoring
- Multi-agent architecture
- Cloud deployment

---

## 👨‍💻 Developer

**Kevin Eliezer DS**

M.Tech — Natural Language Processing

---

## 📄 License

This project is developed for educational and research purposes.
