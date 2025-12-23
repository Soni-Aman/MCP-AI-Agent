
 Multi-Tool AI Assistant using Modern Context Protocol

An **enterprise-grade AI assistant** built using **Modern Context Protocol (MCP)**, **LangChain**, and **Groq LLMs**, 
capable of dynamically orchestrating multiple external tools such as browser automation, web search, and third-party service APIs in a unified, conversational interface.



Features

Multi-Server MCP Integration
  * Playwright MCP (browser automation)
  * DuckDuckGo MCP (web search & intelligence)
  * Airbnb MCP (travel & listing search)

  LLM-Driven Tool Orchestration
  * Powered by Groq’s LLaMA-3.3-70B for high-performance reasoning
  * Autonomous tool selection and execution

  Memory-Enabled Conversational AI
  * Maintains multi-turn conversation context
  * Supports follow-up queries and task chaining

  Schema-Aware Tool Execution
  * Enforced tool argument validation
  * Prevents runtime failures due to malformed function calls

  Real-Time Browser Automation
  * Page navigation, clicks, form filling
  * Screenshots, DOM inspection, and interaction

  Windows-Compatible Deployment
  * NPX-based MCP servers
  * PATH and process spawning fixes for Windows environments

Architecture Overview

```
User
  ↓
MCPAgent (LangChain)
  ↓
Groq LLM (LLaMA-3.3-70B)
  ↓
MCPClient
  ↓
┌───────────────────────────────┐
│ Playwright | DuckDuckGo | Airbnb │
└───────────────────────────────┘
```


Project Structure

mcp-demo/
│
├── browser_mcp.json          # MCP server configuration
├── app.py                   # Memory-enabled MCP chat agent
├── .env                      # Environment variables
├── requirements.txt
└── README.md

 Future Enhancements

 Shopping & price-comparison MCP servers
 SQL & Pandas MCP for data analytics
 Vector database MCP for long-term memory
 Multi-agent coordination
 Monitoring & observability
