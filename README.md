# 🎶 SQL Agent Ollama: Talk to Your Database with LLMs! 🤖

Welcome to **SQL Agent Ollama** — your AI-powered data explorer!  
Ask questions in plain English and let state-of-the-art language models (`llama3.1`, `cogito`, `llama3`) do the SQL heavy lifting on the classic Chinook music database.

---

## 🚀 What is This?

This notebook is a hands-on demo of how you can:
- Connect to a SQLite database (`Chinook.db`)
- Use LangChain’s SQL agent toolkit
- Harness the power of multiple Ollama LLMs
- Query your data with natural language — no SQL expertise needed!

---

## 🛠️ Requirements

- Python 3.8+
- [langchain-community](https://pypi.org/project/langchain-community/)
- [langchain-ollama](https://pypi.org/project/langchain-ollama/)
- [Ollama](https://ollama.com/) (with `llama3.1`, `cogito`, and `llama3` models)
- `Chinook.db` SQLite database file in your project directory

---

## ⚡ Setup

1. **Install dependencies:**
    ```sh
    pip install langchain-community langchain-ollama
    ```

2. **Start Ollama and pull the models:**
    ```sh
    ollama run llama3.1
    ollama run cogito
    ollama run llama3
    ```

3. **Download the Chinook database:**  
   [Get it here](https://github.com/lerocha/chinook-database) and place `Chinook.db` in your project folder.

---

## 📝 How to Use

Open the [`SQL AGENT OLLAMA.ipynb`](c:\Users\ruchita.maaran\Downloads\SQL%20AGENT%20OLLAMA.ipynb) notebook and run the cells step by step.

- **Connect to the database and preview tables**
- **Create a SQL agent with your favorite LLM:**
    ```python
    from langchain_ollama.llms import OllamaLLM
    llm = OllamaLLM(model="llama3.1")  # or "cogito", or "llama3"
    ```
- **Ask your questions in English!**  
  The agent will translate them into SQL, run the queries, and show you the answers.

---

## 💡 Example Questions

- List the total sales per country. Which country's customers spent the most?
- Describe the playlisttrack table.
- List all artists.
- How many albums does Alice in Chains have?
- Find all albums for the artist 'AC/DC'.
- List all tracks in the 'Rock' genre.
- Find the total duration of all tracks.
- How many tracks are there in the album with ID 5?
- Find the total number of invoices.
- Who are the top 5 customers by total purchase?
- Which albums are from the year 2000?
- How many employees are there?

---

## 🌟 Why Use Multiple Models?

Each LLM (`llama3.1`, `cogito`, `llama3`) brings its own strengths.  
Try them all and see which one gives you the best results for your queries!

---

## 📜 License

MIT
---

**Ready to chat with your database? Fire up the
