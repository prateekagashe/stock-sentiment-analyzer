## Project Name: Stock Sentiment Analyzer

## Features

1. Fetch stock code using llm 
2. Fetch stock prices using yfinance
3. Fetch news using Polygon.io
4. Analyze sentiment, people, companies, places, and market implications using an LLM.
5. MLflow integration for prompts, outputs, traces, and metrics.
6. Single-chain workflow using LangChain RunnableLambda.


## Notebook Setup
1. Install Dependencies (Notebook Cell)
All required packages are installed in a notebook cell

2. Configure Environment Variables (Notebook Cell)


## Running the Pipeline

1. Import functions and build the chain:
`chain = stock_prompt_runnable | stock_code_runnable | stock_news_runnable | stock_sentiment_runnable `

2. Invoke the chain for a list of companies:
` result = chain.invoke(['Microsoft', 'Apple Inc', 'Tesla']) `

## MLflow Integration

* Prompts, outputs, and metadata are automatically logged.

* Traces added for:

    1. stock code extraction
    2. News fetching
    3. Sentiment parsing


