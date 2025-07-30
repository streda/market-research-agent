# AI Game Research Agent Project

## Project Overview
UdaPlay is an AI-powered research agent for the video game industry. This project is divided into two main parts that will help build a sophisticated AI agent capable of answering questions about video games using both local knowledge and web searches.

## Project Structure

### Part 1: Offline RAG (Retrieval-Augmented Generation)
In this part, I built a Vector Database using ChromaDB to store and retrieve video game information efficiently.

Key tasks:
- Set up ChromaDB as a persistent client
- Create a collection with appropriate embedding functions
- Process and index game data from JSON files
- Each game document contains:
  - Name
  - Platform
  - Genre
  - Publisher
  - Description
  - Year of Release

### Part 2: AI Agent Development
Built an intelligent agent that combines local knowledge with web search capabilities.

The agent will have the following capabilities:
1. Answer questions using internal knowledge (RAG)
2. Search the web when needed
3. Maintain conversation state
4. Return structured outputs
5. Store useful information for future use

Required Tools to Implement:
1. `retrieve_game`: Search the vector database for game information
2. `evaluate_retrieval`: Assess the quality of retrieved results
3. `game_web_search`: Perform web searches for additional information

## Requirements

### Environment Setup
Create a `.env` file with the following API keys:
```
OPENAI_API_KEY="YOUR_KEY"
CHROMA_OPENAI_API_KEY="YOUR_KEY"
TAVILY_API_KEY="YOUR_KEY"
```

### Project Dependencies
- Python 3.11+
- ChromaDB
- OpenAI
- Tavily
- dotenv


## Testing the Implementation

After completing both parts, I tested agent with questions like:
- "When was Pokémon Gold and Silver released?"
- "Which one was the first 3D platformer Mario game?"
- "Was Mortal Kombat X released for PlayStation 5?"
