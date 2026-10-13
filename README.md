# the company Projects

Internal tooling and data pipelines built during my time as a Data/ML Engineer at a London-based live chat conversion platform (2022–2023) running live chat for 800+ real estate and property clients.

## The system in one line

Live chat transcripts → NLP lead detection → MySQL → Streamlit review dashboard → sales team

## Projects

### Core Pipeline

| Project | What it does |
|---------|-------------|
| [LeadScope UI - final version](./LeadScope%20UI%20-%20final%20version) | Streamlit + Flask dashboard for reviewing and updating lead classifications |
| [Chat data API (Flask)](./Chat%20data%20API%20(Flask)) | REST API serving chat records with date filtering and pagination |
| [LeadScope automation bot (Rasa)](./LeadScope%20automation%20bot%20(Rasa)) | Rasa NLU pipeline — extracts phone/email from chat transcripts to flag leads |
| [Data management CRUD app (Streamlit)](./Data%20management%20CRUD%20app%20(Streamlit)) | Internal admin app for managing the leads database |

### Data Ingestion

| Project | What it does |
|---------|-------------|
| [LiveChat transcripts cron](./LiveChat%20transcripts%20cron) | Automated job pulling closed chat transcripts from LiveChat API into MySQL |
| [LiveChat widget data cron](./LiveChat%20widget%20data%20cron) | Automated job collecting widget interaction events |

### ML & Analysis

| Project | What it does |
|---------|-------------|
| [Bad chat classifier (TensorFlow)](./Bad%20chat%20classifier%20(TensorFlow)) | TensorFlow classifier filtering out spam/bot chats before lead analysis |
| [Word embeddings search (Savills)](./Word%20embeddings%20search%20(Savills)) | Semantic search over a client's knowledge base using sentence-transformers |
| [Proactive vs reactive chats analysis](./Proactive%20vs%20reactive%20chats%20analysis%20(with%20Rohit)) | Conversion rate analysis comparing widget-initiated vs visitor-initiated chats |

### Data Collection

| Project | What it does |
|---------|-------------|
| [Client website scrapers](./Client%20website%20scrapers) | Scrapers for building chat corpora from client websites |
| [Car leasing deals scraper](./Car%20leasing%20deals%20scraper) | Scraper + EDA on UK car leasing listings |

## Tech stack

Python · Flask · Streamlit · Rasa · TensorFlow · MySQL · pandas · sentence-transformers · BeautifulSoup · LiveChat API

## Setup

Each project has its own `README.md`, `requirements.txt`, and `.env.example`. Clone the repo, copy `.env.example` to `.env`, fill in credentials, and follow the project-level README.

```bash
cd <project-folder>
pip install -r requirements.txt
cp .env.example .env
```

> `.env` files are never committed. All credentials live only in your local `.env`.
