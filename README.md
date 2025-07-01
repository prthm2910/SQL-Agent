
# 🧠 LangGraph SQL Agent

This project demonstrates how to build a powerful **SQL Agent** using [LangGraph](https://github.com/langchain-ai/langgraph) and [LangChain](https://github.com/langchain-ai/langchain). It enables an LLM (like OpenAI's GPT models) to interact with a SQL database through multi-step reasoning, tool use, and error correction

---

## 🚀 Features

- 🔍 **Natural Language to SQL**: Ask questions in plain English and get accurate SQL queries generated and executed
- 📊 **Schema-Aware**: Automatically inspects the database schema before querying
- 🧠 **Multi-step Agentic Reasoning**: Uses LangGraph to allow agents to iterate, check, and fix themselves
- 🔁 **Error Correction**: When queries fail, the agent reflects, debugs, and retries

---

## 🧰 Tech Stack

| Tool        | Purpose                                 |
|-------------|------------------------------------------|
| LangGraph   | Agent state machine and workflow engine |
| LangChain   | LLM framework with SQL support tools     |
| SQLite      | Lightweight embedded SQL database        |
| Python      | Core programming language                |
| OpenAI API  | Language model backend                   |


---

## Workflow

![SQL Agent Workflow](SQL - Agent Workflow Diagram.png)

---

## 📁 File Structure

```
├── sql-agent.ipynb        # Main tutorial notebook
├── requirements.txt       # Python dependencies (if available)
└── README.md              # You're here!
```

---

## 📦 Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/sql-agent.git
   cd sql-agent
   ```

2. **Install Dependencies**
   You can use `pip` or a virtual environment:
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure Environment Variables**
   Set your OpenAI API Key:
   ```bash
      OPENAI_API_KEY=your-key-here    
   ```


---

## 📝 Example Prompts

- "What is the average salary in the employees table?"
- "List all customers who made a purchase in the last 30 days"
- "How many orders were placed in each region?"

---

## ⚠️ Limitations

- Currently supports **read-only** SQL operations (i.e., `SELECT`)
- For `INSERT`, `UPDATE`, or `DELETE`, you'd need to build custom tools

---

## 🧩 Extending the Project

- Build custom LangChain tools for SQL `INSERT`, `UPDATE`, etc.
- Integrate schema validation for safer write operations
- Add UI with Streamlit

---

