🎶 SQL Agent Ollama: Talk to Your Database with LLMs! 🤖
Welcome to SQL Agent Ollama — your AI-powered data companion!
This project lets you interact with your database using natural language. Whether you're a data analyst, developer, or just curious, you can skip writing SQL and let cutting-edge Large Language Models (LLMs) do the work for you.

Powered by Ollama, LangChain, and the Chinook music database — this tool turns simple English into real SQL queries and answers.

🚀 What is SQL Agent Ollama?
This project demonstrates how to:

🔌 Connect to a local SQLite database (Chinook.db)

🧠 Leverage LangChain’s SQL Agent with Ollama-hosted LLMs

💬 Query data by typing plain English, no SQL knowledge required

You can interactively explore a real-world music database using models like:

llama3.1

cogito

llama3

It’s perfect for learning, prototyping, or just having fun with AI-powered data queries.

🛠️ Prerequisites
Before you begin, make sure you have the following installed:

Python 3.8 or later

langchain-community

langchain-ollama

Ollama with required models

The Chinook.db SQLite database (see below)

⚙️ Setup Instructions
1. Install the required Python packages:
sh
Copy
Edit
pip install langchain-community langchain-ollama
2. Start Ollama and pull the models:
Make sure Ollama is installed and running, then execute:

sh
Copy
Edit
ollama run llama3.1
ollama run cogito
ollama run llama3
ℹ️ These commands will download and spin up each model. You can experiment with each to compare their performance.

3. Get the Chinook Database:
Download the database from the Chinook GitHub repository and place the Chinook.db file in your project directory.

🧪 How to Use the Notebook
Open the Jupyter Notebook file:
📄 SQL AGENT OLLAMA.ipynb

(Path shown in the original: c:\Users\ruchita.maaran\Downloads\SQL%20AGENT%20OLLAMA.ipynb — make sure the file is accessible from your working directory)

Then, follow these steps:

Load the database and inspect its structure

Choose an LLM and initialize the SQL agent
Example:

python
Copy
Edit
from langchain_ollama.llms import OllamaLLM
llm = OllamaLLM(model="llama3.1")  # or "cogito", or "llama3"
Ask your questions in English
The agent will convert them to SQL queries and show the results instantly.

💬 Sample Questions You Can Ask
Here are some example queries to try out:

“List the total sales per country. Which country’s customers spent the most?”

“Describe the playlisttrack table.”

“List all artists.”

“How many albums does Alice in Chains have?”

“Find all albums for the artist AC/DC.”

“List all tracks in the ‘Rock’ genre.”

“What is the total duration of all tracks?”

“How many tracks are there in the album with ID 5?”

“Find the total number of invoices.”

“Who are the top 5 customers by total purchase?”

“Which albums were released in the year 2000?”

“How many employees are there?”

Feel free to explore further — the database is rich with data!

🌐 Why Multiple Models?
Each LLM has unique capabilities:

Model	Strengths
llama3.1	Fast and general-purpose, great for SQL conversion
cogito	May offer more nuanced understanding of edge cases
llama3	Smaller and faster, useful for lightweight tasks

🔍 Try asking the same question to different models and compare the outputs!

📜 License
This project is licensed under the MIT License — feel free to modify, use, or extend it however you like.

✅ Ready to Chat with Your Database?
Start the notebook and talk to your data today — no SQL required! 🎧📊
