# News Summarizer Agent

> Transform news articles into structured, AI-powered briefings.

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![LangChain](https://img.shields.io/badge/LangChain-Framework-green.svg)](https://www.langchain.com/)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4o--mini-black.svg)](https://openai.com/)
[![NewsAPI](https://img.shields.io/badge/NewsAPI-Optional-orange.svg)](https://newsapi.org/)

News Summarizer Agent is an AI-powered information processing agent that retrieves news articles on a specified topic and generates concise, structured briefings.

Built with **LangChain** and **OpenAI GPT-4o-mini**, the agent analyzes news content, identifies key themes, extracts important insights, and produces an organized summary of the latest information.

It supports both live news retrieval through **NewsAPI** and built-in mock data for testing and development without requiring external API credentials.

---

## ✨ Key Features

* 📰 Retrieve news articles based on any topic
* 🧠 Generate AI-powered structured summaries
* 🔍 Identify key themes and important insights
* 📊 Configure the number of articles to analyze
* 🌐 Support real-time news retrieval with NewsAPI
* 🧪 Run locally with built-in mock data
* 🔑 Operate without external API keys in demo mode
* ⚡ Simple command-line interface
* 📋 Generate structured news briefings

---

## 🚀 Quick Start

### Requirements

Before getting started, make sure you have:

* Python 3.10 or later
* OpenAI API key
* NewsAPI key *(optional)*

### Installation

Clone the repository:

```bash
git clone <repository-url>
cd news-summarizer-agent
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Create your environment configuration:

```bash
cp .env.example .env
```

Configure your API keys:

```env
OPENAI_API_KEY=your_openai_api_key
NEWS_API_KEY=your_newsapi_key
```

> The NewsAPI key is optional. The agent can run using built-in mock data for testing and development.

---

## 💡 Usage

### Summarize News on a Topic

```bash
python agent.py --topic "artificial intelligence"
```

### Configure the Number of Articles

```bash
python agent.py \
  --topic "climate change" \
  --count 10
```

---

## 🧪 Mock Data Mode

The agent includes built-in sample news data, allowing you to test the summarization workflow without a NewsAPI key.

This makes the project useful for:

* Local development
* Testing
* Demonstrations
* Learning AI agent workflows

For live news retrieval, configure a valid NewsAPI key in your `.env` file.

---

## 🧠 How It Works

```text
Topic
  │
  ▼
┌─────────────────────────────┐
│ News Article Retrieval      │
│ NewsAPI / Mock Data         │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│ Content Processing           │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│ LangChain + GPT-4o-mini     │
│ AI Content Analysis          │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│ Theme & Insight Extraction   │
└──────────────┬──────────────┘
               │
               ▼
      Structured News Briefing
```

---

## 📊 Generated Intelligence

The agent analyzes retrieved articles and generates structured information including:

* Concise article summaries
* Key themes
* Important insights
* Major developments
* Topic-level synthesis
* Structured news briefings

---

## 🏗️ Tech Stack

| Component      | Technology          |
| -------------- | ------------------- |
| Language       | Python              |
| LLM Framework  | LangChain           |
| Language Model | OpenAI GPT-4o-mini  |
| News Retrieval | NewsAPI             |
| Data Source    | NewsAPI / Mock Data |
| Interface      | Command Line        |

---

## 🎯 Use Cases

News Summarizer Agent can serve as a foundation for:

* AI research assistants
* News monitoring systems
* Market intelligence tools
* Industry monitoring agents
* Automated briefing systems
* Competitive intelligence platforms
* Research and information synthesis tools
* Intelligence dashboards

---

## 🔮 Future Improvements

Planned improvements include:

* Support for additional news sources
* Article deduplication
* Source credibility scoring
* Multilingual news summarization
* Web interface
* Scheduled news briefings
* Historical summary storage
* Trend analysis across time
* Personalized news monitoring
* Email and Slack briefing delivery

---

## 🤝 Contributing

Contributions, ideas, and feedback are welcome.

To contribute:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test your implementation
5. Submit a pull request

---

## 🔐 Security and Privacy

News content and API credentials should be handled responsibly.

* Never commit API keys to the repository.
* Store credentials in environment variables.
* Use `.env.example` for configuration templates.
* Review the terms and usage limits of external news providers.
* Consider privacy and licensing requirements when storing or redistributing article content.

---

## 📄 License

This project is licensed under the MIT License.

See the `LICENSE` file for more information.
