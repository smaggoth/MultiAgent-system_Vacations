# 🌍 AI Multi-Agent Vacation Planner

This project implements **multi-agent orchestration** system using **LangGraph** and **LangChain**. The system is designed to take a user's seasonal preference and travel dates to generate a complete vacation plan.

## 🤖 Agents & Roles
- **Manager Agent:** The "brain" of the operation. Orchestrates the workflow and ensures the global state is updated.
- **Destination Agent:** Researches the best locations based on the season powered by MCP to search thru the web.
- **Flight Agent:** Finds the best flight options for the selected destination and date powered by traveler MCP server.
- **Hotel Agent:** Searches for accommodations and lodging also using the MCP web.

## 🛠️ Tech Stack
- **Framework:** LangChain & LangGraph
- **LLM Engine:** Ollama (Qwen 2.5/3-VL)
- **State Management:** Custom State Schemas with Persistence.
- **Tools:** Custom Python Tools for web search and state updates.

## 🚀 Key Features
- **Deterministic State Updates:** Ensures all required data (date, season, destination) is saved before proceeding.
- **Tool-Calling Orchestration:** Robust handling of agent handoffs.
- **Local LLM Support:** Optimized for running with local models.
