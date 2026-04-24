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
