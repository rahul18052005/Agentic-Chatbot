# 🤖 End-to-End Agentic AI Chatbot and Chatbot with WebSearch



An **End-to-End Agentic AI Chatbot and Chatbot with WebSearch** built using **Python, LangGraph, LLMs, Web Search, and Streamlit**.

This chatbot can understand user queries, decide whether web search is required, use a web-search tool to retrieve relevant information, and generate a final response using an LLM.

---

## 🚀 Features

- 🤖 AI-powered conversational chatbot
- 🧠 Agentic workflow using LangGraph
- 🌐 Web search for real-time information
- 🔧 Tool calling
- 🔄 State-based workflow
- 💬 Interactive Streamlit chat interface
- ⚡ AI-generated responses based on retrieved information

---

## 🧠 How It Works

The application follows an agentic workflow where the user's query is first processed by the AI agent.

The agent analyzes the query and decides whether it can answer directly using the LLM or whether it needs additional information from the web.

If web search is not required, the query is directly processed by the LLM and the response is returned to the user.

If web search is required, the agent calls the web-search tool, retrieves relevant information, processes the search results, and sends the required context to the LLM. The LLM then generates the final response based on the retrieved information.

### Workflow

```text
User
 │
 ▼
User Query
 │
 ▼
Agent / LangGraph
 │
 ▼
Query Analysis
 │
 ├─────────────── No ───────────────► LLM
 │                                     │
 │                                     ▼
 │                              Final Response
 │
 └─────────────── Yes
                       │
                       ▼
                  Web Search
                       │
                       ▼
                 Search Results
                       │
                       ▼
                 LLM Processing
                       │
                       ▼
                 Final Response
                       │
                       ▼
                  Streamlit UI
```


## 📂 Project Structure

```text
Agentic-AI-Chatbot/
│
├── src/
│   ├── langgraph/
│   │   ├── graph/
│   │   ├── LLMs/
│   │   ├── nodes/
│   │   ├── state/
│   │   ├── tools/
│   │   ├── ui/
│   │   ├── main.py
│   │   └── __init__.py
│   │
│   └── __init__.py
│
├── app.py
├── requirements.txt
├── .gitignore
└── README.md
```

---

## 🛠️ Tech Stack

| **Python** | Core programming language |
| **LangGraph** | Agent workflow and state management |
| **LLM** | Natural language understanding and response generation |
| **Web Search** | Retrieving current information from the web |
| **Streamlit** | Interactive chatbot interface |
| **Git & GitHub** | Version control and project management |

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/rahul18052005/Agentic-Chatbot.git
```

```bash
cd agentic-chatbot
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

### 3. Activate the Environment

#### Windows

venv\Scripts\activate


### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

---

```gitignore
venv/
__pycache__/
*.pyc
```

---

## ▶️ Run the Application

Run the Streamlit application using:

```bash
streamlit run app.py
```

After running the command, open the URL displayed in the terminal.

Usually:

```text
http://localhost:8501
```

---

## 💬 Example Queries

### General Query

```text
What is LangGraph?
```

### AI Query

```text
Explain Agentic AI in simple terms.
```

### Web Search Query

```text
What are the latest developments in AI Agents?
```

### Research Query

```text
Search the web for the latest RAG frameworks.
```

---

## 🎯 Use Case

This project demonstrates how **LLMs, Agentic AI, LangGraph, tool calling, and web search** can be combined to build an intelligent AI assistant capable of retrieving external information when required.

It can be used as a foundation for building more advanced **AI agents, research assistants, and intelligent search applications**.

---

## 👨‍💻 Author

**Rahul Hor**

**Computer Science Engineering Student | AI/ML & Generative AI Enthusiast**

---

