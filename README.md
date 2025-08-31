# LLM Web Search

AI-powered web search that scrapes real-time content and provides accurate answers using Google Gemini.

## Features

- **Web Search** - Google Serper API integration
- **Content Scraping** - BeautifulSoup extraction
- **AI Answers** - Google Gemini responses based on scraped data
- **Streamlit UI** - Clean web interface
- **Token Tracking** - Usage statistics
- **Content Logging** - Timestamped storage

## Quick Start

```bash
git clone https://github.com/ashish-gfg/llm_search.git
cd llm_search
pip install -r requirements.txt
```

Create `.env` file:
```env
SERPER_API_KEY=your_key
GEMINI_API_KEY=your_key
```

Run:
```bash
streamlit run client.py
```

## Docker

```bash
docker build -t llm-search .
docker run -p 8501:8501 -e SERPER_API_KEY=key -e GEMINI_API_KEY=key llm-search
```

## API Keys

- [Google Serper](https://serper.dev) - Web search
- [Google Gemini](https://makersuite.google.com/app/apikey) - AI responses

## How It Works

1. Search web for relevant links
2. Scrape content from multiple sources  
3. Combine into comprehensive context
4. AI generates answer based only on scraped data
5. Display with token usage stats
