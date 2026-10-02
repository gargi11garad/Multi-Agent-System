# Multi-Agent-System
An AI-powered multi-agent research system that uses Search, Reader, Writer, and Critic agents to automatically collect information, analyze sources, generate reports, and review them.  Built using Python, LangChain, Tavily, OpenRouter, and Streamlit.
# 🤖 Multi-Agent AI Research System

An **AI-powered multi-agent research system** that automates web research, content extraction, report generation, and report evaluation using specialized AI agents.

## 🚀 Features

* 🔍 **Search Agent** – Finds recent and reliable information using Tavily.
* 📖 **Reader Agent** – Scrapes relevant web pages for detailed content.
* ✍️ **Writer Agent** – Generates a structured research report.
* 🧐 **Critic Agent** – Reviews the report and provides feedback.
* 🖥️ **Streamlit UI** – Simple interface to enter topics and view results.
* 🔗 **LLM Integration** – Uses an LLM through OpenRouter.

## 🏗️ Architecture

```text
             User
               │
               ▼
        ┌──────────────┐
        │  Streamlit UI │
        └──────┬───────┘
               │
               ▼
        ┌──────────────┐
        │ Search Agent │
        └──────┬───────┘
               │
               ▼
        ┌──────────────┐
        │ Reader Agent │
        └──────┬───────┘
               │
               ▼
        ┌──────────────┐
        │ Writer Agent │
        └──────┬───────┘
               │
               ▼
        ┌──────────────┐
        │ Critic Agent │
        └──────────────┘
               │
               ▼
        Research Report
```

## 🛠️ Tech Stack

* Python
* LangChain
* OpenRouter
* Tavily
* BeautifulSoup
* Streamlit
* python-dotenv

## 📂 Project Structure

```text
multi-agent-system/
│
├── agents.py          # AI agents and LLM configuration
├── tools.py           # Web search and scraping tools
├── pipeline.py        # Research pipeline
├── app.py             # Streamlit application
├── .env               # API keys
├── .gitignore
└── README.md
```

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/multi-agent-system.git
cd multi-agent-system
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it:

**Windows:**

```bash
.venv\Scripts\activate
```

**Linux/macOS:**

```bash
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure API keys

Create a `.env` file:

```env
OPENROUTER_API_KEY=your_openrouter_api_key
TAVILY_API_KEY=your_tavily_api_key
```

> ⚠️ Never commit your `.env` file or expose your API keys on GitHub.

## ▶️ Run the Project

### Run from terminal

```bash
python pipeline.py
```

### Run Streamlit UI

```bash
python -m streamlit run app.py
```

Then open the local Streamlit URL shown in your terminal.

## 🔄 Workflow

1. User enters a research topic.
2. **Search Agent** searches the web.
3. **Reader Agent** extracts detailed information from relevant sources.
4. **Writer Agent** generates the research report.
5. **Critic Agent** evaluates the report.
6. Results are displayed through the Streamlit interface.

## 🎯 Example

**Input:**

```text
Artificial Intelligence in Healthcare
```

**Output:**

* Search results
* Detailed scraped content
* Structured research report
* Critic feedback and score

## 🔮 Future Improvements

* Add more specialized research agents.
* Support multiple research sources simultaneously.
* Add PDF/document research.
* Add report export to PDF/DOCX.
* Improve source verification and citation handling.
* Add conversation history and persistent research sessions.

## 👩‍💻 Author

**Gargi Garad**

---

⭐ If you find this project useful, consider giving it a star on GitHub.
