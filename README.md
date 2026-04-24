# AI News Aggregator

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Docker](https://img.shields.io/badge/Docker-Containerized-blue)
![LLM](https://img.shields.io/badge/LLM-Local-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

An autonomous AI-powered news aggregator that fetches articles 
from NewsAPI, summarizes them using a local LLM, and delivers 
a clean daily email digest automatically.

---

## Features

- Fetches latest news from NewsAPI across topics like AI, tech, science
- Summarizes articles using a local LLM — no OpenAI costs
- Compiles summaries into a structured daily email digest
- Fully containerized with Docker for easy deployment
- Stores articles in PostgreSQL for deduplication

---

## Tech Stack

| Component | Technology |
|---|---|
| Language | Python 3.11 |
| News Source | NewsAPI |
| Summarization | Local LLM |
| Email Delivery | SMTP |
| Database | PostgreSQL |
| Containerization | Docker |

---

## Project Structure
ai-news-aggregator/
├── app/
│   ├── fetcher.py        # Fetches articles from NewsAPI
│   ├── summarizer.py     # Summarizes using local LLM
│   ├── digest.py         # Compiles daily digest
│   └── emailer.py        # Sends email automatically
├── docker/
│   └── Dockerfile
├── main.py               # Entry point
├── pyproject.toml
├── .env.example
└── README.md
1. Fetches latest articles from NewsAPI
2. Passes each article to local LLM for 2-3 line summary
3. Compiles all summaries into structured digest
4. Sends digest to inbox automatically every day

---

## What I Learned

- Building autonomous end-to-end AI pipelines
- Integrating local LLMs for cost-free summarization
- Automating data ingestion, processing and delivery
- Docker containerization for reproducible deployment
- Real-world debugging and iterative development

---

## License

MIT License

