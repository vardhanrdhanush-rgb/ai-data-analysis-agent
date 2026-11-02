# AI Data Analysis Agent

An **AI-powered data analysis agent** that lets you ask plain-English questions about any CSV or Excel file and get back computed answers, summaries, and insights — no SQL or pandas code needed.

## What it does

- Upload any CSV or Excel file
- Ask questions in plain English: "What is the average revenue by region?" or "Which customers churned in Q3?"
- The agent writes and executes DuckDB SQL or pandas queries internally to compute the answer
- Returns the result in natural language with supporting data

## Tech stack

| Component | Tool |
|---|---|
| Agent | Agno (OpenAI GPT-4o) |
| Query engine | DuckDB + pandas |
| File support | CSV, Excel (.xlsx) |
| UI | Streamlit |

## Setup

```bash
pip install -r requirements.txt
export OPENAI_API_KEY=your_key
streamlit run ai_data_analyst.py
```

## Example questions

- "Show me the top 10 rows sorted by sales descending"
- "What's the monthly trend in customer sign-ups?"
- "Are there any null values in the dataset? Which columns?"
- "Calculate the year-over-year growth rate for each product category"

## Skills demonstrated

- Agentic data analysis with tool-using LLMs
- Pandas and DuckDB for tabular data processing
- ETL pipeline patterns (ingest, clean, transform, analyze)
- Streamlit application development
- Handling real-world messy data (mixed types, nulls, date parsing)
