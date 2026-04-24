AI News Aggregator
An autonomous AI-powered news aggregator that fetches articles from NewsAPI, summarizes them using a local LLM, and delivers a clean daily email digest automatically.
What It Does

Fetches latest news articles from NewsAPI across categories like technology, AI, and science
Summarizes each article using a local LLM — no OpenAI API key required
Compiles summaries into a structured daily digest
Sends the digest automatically via email every day

Project Structure
ai-news-aggregator/
├── app/
│   ├── fetcher.py        # Fetches articles from NewsAPI
│   ├── summarizer.py     # Summarizes articles using local LLM
│   ├── digest.py         # Compiles daily email digest
│   └── emailer.py        # Sends digest via email
├── docker/
│   └── Dockerfile        # Docker configuration
├── main.py               # Entry point — runs daily pipeline
├── pyproject.toml        # Dependencies
├── .env.example          # Environment variables template
└── README.md
Tech Stack

Python — core language
NewsAPI — news article fetching
Local LLM — article summarization without external API costs
SMTP — automated email delivery
Docker — containerized deployment
PostgreSQL — article storage and digest management

Setup
1. Clone the repository
bashgit clone https://github.com/ArnavGulkari/ai-news-aggregator.git
cd ai-news-aggregator
2. Create environment file
bashcp .env.example .env
3. Add your credentials to .env
NEWSAPI_KEY=your_newsapi_key
EMAIL_SENDER=your_email@gmail.com
EMAIL_PASSWORD=your_app_password
EMAIL_RECEIVER=receiver@gmail.com
4. Install dependencies
bashpip install -r requirements.txt
5. Run the pipeline
bashpython main.py
Or run with Docker:
bashdocker compose up
How It Works

fetcher.py calls NewsAPI and retrieves latest articles
summarizer.py passes each article to a local LLM and generates a 2-3 line summary
digest.py compiles all summaries into a structured daily digest
emailer.py sends the digest to your inbox automatically

Deployment
The project supports three deployment stages:

Local — run directly with Python
Docker — containerized for consistent environments
Production — scheduled daily pipeline with logging

What I Learned

Building end-to-end autonomous AI pipelines
Integrating local LLMs for cost-free summarization
Automating data ingestion, processing, and delivery workflows
Docker containerization for reproducible deployments
Real-world debugging and iterative development

License
MIT License
