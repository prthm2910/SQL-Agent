
# 🧠 LangGraph SQL Agent Tutorial

This project demonstrates how to build a powerful **SQL Agent** using [LangGraph](https://github.com/langchain-ai/langgraph) and [LangChain](https://github.com/langchain-ai/langchain). It enables an LLM (like OpenAI's GPT models) to interact with a SQL database through multi-step reasoning, tool use, and error correction.

---

## 🚀 Features

- 🔍 **Natural Language to SQL**: Ask questions in plain English and get accurate SQL queries generated and executed.
- 📊 **Schema-Aware**: Automatically inspects the database schema before querying.
- 🧠 **Multi-step Agentic Reasoning**: Uses LangGraph to allow agents to iterate, check, and fix themselves.
- 🔁 **Error Correction**: When queries fail, the agent reflects, debugs, and retries.

---

## 🧰 Tech Stack

| Tool        | Purpose                                 |
|-------------|------------------------------------------|
| LangGraph   | Agent state machine and workflow engine |
| LangChain   | LLM framework with tools for SQL         |
| SQLAlchemy  | Database access abstraction layer        |
| SQLite      | Example SQL database (can be swapped)    |
| Python      | Core programming language                |
| OpenAI API  | Language model backend                   |

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
   git clone https://github.com/your-username/sql-agent-tutorial.git
   cd sql-agent-tutorial
   ```

2. **Install Dependencies**
   You can use `pip` or a virtual environment:
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure Environment Variables**
   Set your OpenAI API Key:
   ```bash
   export OPENAI_API_KEY=your-key-here  # For Linux/macOS
   set OPENAI_API_KEY=your-key-here     # For Windows
   ```

4. **Launch the Notebook**
   ```bash
   jupyter notebook sql-agent.ipynb
   ```

---

## 📝 Example Prompts

- "What is the average salary in the employees table?"
- "List all customers who made a purchase in the last 30 days."
- "How many orders were placed in each region?"

---

## ⚠️ Limitations

- Currently supports **read-only** SQL operations (i.e., `SELECT`).
- For `INSERT`, `UPDATE`, or `DELETE`, you'd need to build custom tools.

---

## 🧩 Extending the Project

Want to add write capabilities? You can:
- Build custom LangChain tools for SQL `INSERT`, `UPDATE`, etc.
- Integrate schema validation for safer write operations.
- Add UI with Streamlit or Gradio.

---

## 🤝 Contributing

Contributions, bug reports, and ideas are welcome! Please open an issue or PR.

---

## 📄 License

This tutorial is open-sourced under the MIT License.

---

## 🌐 Credits

Developed with ❤️ using LangGraph and LangChain.
