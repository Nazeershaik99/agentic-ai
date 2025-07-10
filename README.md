# 🧠 Non-Linear Agent Using LangGraph + Mistral via Ollama

A smart, dynamic AI agent built using [LangGraph](https://github.com/langchain-ai/langgraph), powered by [Mistral LLM](https://mistral.ai) and served locally via [Ollama](https://ollama.com). This agent leverages a **non-linear execution graph** to perform advanced multi-step reasoning, tool usage, and memory-based decision-making.

---

## 🚀 Project Overview

Traditional agents follow a linear sequence of steps. In contrast, this project demonstrates a **non-linear agent architecture** using **LangGraph**, enabling:

- Branching decisions based on output
- Tool invocation logic
- Stateful memory handling
- Looping, conditional execution, and complex flow

All powered by the **Mistral** language model hosted locally with **Ollama**.

---

## 🛠️ Tech Stack

| Layer          | Technology         |
|----------------|--------------------|
| Language Model | [Mistral](https://mistral.ai) via [Ollama](https://ollama.com) |
| Graph Engine   | [LangGraph](https://github.com/langchain-ai/langgraph) |
| Agent Framework| [LangChain](https://www.langchain.com) |
| Programming    | Python |
| Tools          | Built-in LangChain tools or custom tools (e.g., Math, Search, Python REPL) |

---

## 📌 Features

- 🧭 **Non-linear Agent Routing** using LangGraph nodes
- 🧠 **LLM-Driven Decisions** powered by Mistral
- 🔁 **Conditional Loops and Memory** (Conversation history, results caching)
- 🧰 **Tool Calling Support** (e.g., Search, Calculator, Python REPL)
- ⚡ **Runs Fully Local** with Ollama + Mistral
- 🧪 **Extendable**: Add custom tools, memory modules, and branches

---

## 📂 Project Structure

```bash
nonlinear-agent/
│
├── main.py                # Entry point
├── agent_graph.py         # LangGraph flow definition
├── tools.py               # Custom and built-in tool definitions
├── memory.py              # Optional: memory integration
├── requirements.txt       # Python dependencies
├── README.md              # This file
└── .env                   # Optional: env vars (API keys, etc.)


🔧 Setup Instructions
1. Install Ollama & Pull Mistral
curl -fsSL https://ollama.com/install.sh | sh
ollama run mistral

2. Clone the Repository
git clone https://github.com/yourusername/nonlinear-agent.git
cd nonlinear-agent


3. Create Virtual Environment & Install Requirements
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt


4. Run the Agent
python main.py


🤖 Architecture Diagram
[User Input]
     ↓
[LangGraph Node: Input Handler]
     ↓
[LangGraph Node: Decide → Tool? → Memory? → End?]
     ↙         ↓        ↘
[Tool Node] [Memory Node] [Final Output]
     ↓         ↓            ↑
    Loop back to decision if needed


🌐 References
LangGraph Documentation
Ollama + Mistral Setup
LangChain Agents

🙋‍♂️ Author
Made by Shaik Nazeer
