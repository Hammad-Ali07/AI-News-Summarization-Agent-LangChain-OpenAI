# News Summarizer Agent

An AI-powered news summarization agent that collects articles on a specified topic and generates a structured briefing with key themes, important insights, and concise summaries.

The project demonstrates how to build an intelligent information-processing workflow using **LangChain** and **GPT-4o-mini**, with optional integration with **NewsAPI** for real-time news retrieval.

## Features

* Fetches news articles based on any topic
* Generates structured AI-powered summaries
* Identifies key themes and important insights
* Supports configurable article counts
* Works with real NewsAPI data or built-in mock data
* Runs without an API key for testing and development
* Simple command-line interface

## Tech Stack

* **Framework:** LangChain
* **LLM:** GPT-4o-mini
* **News Data:** NewsAPI *(optional)*
* **Language:** Python

## Installation

Clone the repository and install the required dependencies:

```bash
pip install -r requirements.txt
```

Create your environment configuration file:

```bash
cp .env.example .env
```

Add your NewsAPI key to the `.env` file if you want to retrieve live news articles.

## Usage

Run the agent with a topic:

```bash
python agent.py --topic "artificial intelligence"
```

Specify the number of articles to analyze:

```bash
python agent.py --topic "climate change" --count 10
```

## Mock Data Mode

The agent can run without a NewsAPI key using built-in sample data. This makes the project easy to test locally without requiring external API credentials.

For real-time news data, obtain a free API key from NewsAPI and configure it in your `.env` file.

## Example Workflow

```text
Topic
  ↓
News Article Retrieval
  ↓
Content Processing
  ↓
AI Analysis
  ↓
Theme Extraction
  ↓
Structured News Briefing
```

## Project Purpose

This project demonstrates the practical application of **LLM-powered agents for information retrieval, content analysis, and structured knowledge synthesis**. It can serve as a foundation for more advanced systems such as research assistants, monitoring agents, intelligence dashboards, and automated briefing tools.

## Future Improvements

* Add support for additional news sources
* Implement article deduplication
* Add source credibility scoring
* Support multilingual news summarization
* Add a web interface
* Implement scheduled news briefings
* Store historical summaries for trend analysis


