# 🚀 Natural Language SQL Agent with IBM Granite

![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python)
![IBM](https://img.shields.io/badge/IBM-Watsonx.ai-be95ff?style=for-the-badge&logo=ibm)
![LangChain](https://img.shields.io/badge/LangChain-Framework-121212?style=for-the-badge&logo=chainlink)
![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql)

## 📝 Project Overview
In the modern business landscape, extracting insights from SQL databases often requires specialized technical knowledge. This project solves that challenge by building an **AI-powered system** that converts everyday natural language into MySQL queries.

By using the **IBM Granite-3-2-8b-instruct** model and **LangChain**, users can simply ask questions like *"How many albums are there?"* and receive instant, accurate answers directly from the data.

[Image of the entity relationship diagram for the Chinook database]

## 🛠️ Core Objectives
* **Integrate NLP**: Leverage IBM Watsonx to interpret complex natural language queries.
* **Automated SQL Execution**: Translate questions into SQL syntax to fetch data from the MySQL database.
* **Intelligent Error Recovery**: Use a SQL agent that can capture tracebacks and regenerate queries if necessary.

## 📊 Database Schema: The Chinook Database
The project queries the **Chinook database**, which models a digital media store ecosystem:
* **Interconnected Tables**: Includes 11 distinct tables like Artist, Album, Track, and Invoice.
* **Rich Dataset**: Contains over 15,000 records, including authentic media data and realistic sales records.

## 📁 Project Structure
| File | Description |
| :--- | :--- |
| **`llm_agent.py`** | Tests the Watsonx model connection with a sample geographical query. |
| **`sql_agent.py`** | The main script containing the LangChain SQL Agent and MySQL connector. |
| **`chinook-mysql.sql`** | The SQL source file

---

## 💻 Setup & Usage
1.  **Activate Environment**:
    ```bash
    source my_env/bin/activate
    ```
2.  **Run the Agent**:
    ```bash
    python3 sql_agent.py --prompt "How many Album are there in the database?"
    ```

## 🎯 Sample Result
When queried about the media catalog, the agent produces a detailed "Thought" process:
> **Final Answer:** There are 347 Albums in the database.

---

## 👤 Author
**Leelaissak Attota**
* **Email**: attotaleelaissak@gmail.com
* **Project Context**: Built as part of the IBM Skills Network "Build a Natural Language SQL Agent" project.
