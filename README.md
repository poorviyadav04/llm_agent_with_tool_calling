# LangChain Tool-Using AI Agent

This project demonstrates a **tool-using AI agent** built with LangChain that runs a **local LLM via Ollama**.  
The agent performs multi-step reasoning and dynamically calls tools to answer user questions.

## Features

- Tool calling with LangChain
- Manual agent loop implementation
- Local LLM inference using Ollama
- Execution tracing with LangSmith

## Tools

- **get_product_price** – retrieves product price from a catalog  
- **apply_discount** – applies a discount tier to a price

## Example

Question:

What is the price of a laptop after applying a gold discount?

Agent workflow:


User question
↓
Call get_product_price
↓
Call apply_discount
↓
Return final answer


## Run

Install dependencies:


pip install -r requirements.txt


Run the agent:


python main.py


Make sure Ollama is running and the model is installed:


ollama pull qwen3:1.7b


## Tech Stack

- Python
- LangChain
- Ollama
- LangSmith