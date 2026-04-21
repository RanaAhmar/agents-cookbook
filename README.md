# AI Agents Cookbook 🤖👨‍🍳

[![Sponsored by Stackaura](https://img.shields.io/badge/Sponsored_by-Stackaura-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://www.stackaura.com/)
[![Agents](https://img.shields.io/badge/AI_Agents-Cookbook-ff69b4.svg?style=for-the-badge)](https://www.stackaura.com/)

A practical, hands-on collection of recipes, architectures, and boilerplate code to build advanced AI Agents. Stop wrestling with theory and start building reliable, autonomous systems.

---

<div align="center">
  <h3>Sponsored by <a href="https://www.stackaura.com/">Stackaura</a></h3>
  <p>Accelerating agentic AI development and complex workflow automation.</p>
  <a href="https://www.stackaura.com/"><img src="https://img.shields.io/badge/Visit_Stackaura-Black?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Visit Stackaura" /></a>
</div>

---

## 🍳 What's Cooking?

The landscape of AI is shifting from static chat interfaces to autonomous agents that can plan, execute tools, and solve complex multi-step problems. This cookbook provides the essential ingredients and recipes to build your own agents using leading frameworks.

## 🥘 Recipes Included

### 1. The Basics: Tool Use
How to give your LLM hands and eyes.
- Simple calculator agent
- Web searching agent
- API interacting agent

### 2. Multi-Agent Systems
When one bot isn't enough.
- **The Debate Model**: Two agents arguing to find the truth.
- **Hierarchical Crews**: A manager agent orchestrating worker agents (using CrewAI / AutoGen).

### 3. Memory & State Management
Giving your agents a brain that remembers.
- Implementing Redis for short-term conversation state.
- Integrating Vector DBs (Chroma/Pinecone) for long-term semantic memory.

### 4. Evaluation & Tracing
How to figure out *why* your agent did that weird thing.
- Setting up LangSmith / Phoenix traces.
- Prompt evaluation pipelines.

## 🛠️ Frameworks Covered

We provide parallel examples using the most popular modern frameworks:
- **LangChain / LangGraph**: For complex, stateful workflows.
- **LlamaIndex**: Fast, data-connected specialized agents.
- **CrewAI / AutoGen**: For collaborative multi-agent simulation.

## 💻 Quick Start Example

A taste of what's inside (Simple Tool-Calling Agent using LangChain):

```python
from langchain_openai import ChatOpenAI
from langchain.agents import initialize_agent, AgentType
from tools import search_web, calculate

llm = ChatOpenAI(temperature=0, model="gpt-4-turbo")
tools = [search_web, calculate]

agent = initialize_agent(
    tools, 
    llm, 
    agent=AgentType.OPENAI_FUNCTIONS, 
    verbose=True
)

agent.run("What is the current population of Tokyo multiplied by 2?")
```

## 🤝 Contributing

We want your recipes! If you've built a clever agent architecture or solved a tricky memory problem, please contribute!
1. Fork the repository
2. Add your recipe to the appropriate folder
3. Ensure it runs and includes requirements
4. Open a pull request

## 📜 Notice

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
*Architected and maintained by the AI engineering team at [Stackaura](https://www.stackaura.com/).*


---

## 🚀 Discover More from Stackaura

If you found this tool useful, check out our other high-performance web utilities and follow **Ahmar Hussain** for more open-source excellence.

### 🌟 Featured Projects
- **[Free LLM APIs](https://github.com/RanaAhmar/free-llm-apis)** - A curated list of zero-cost AI endpoints.
- **[Awesome MCP Servers](https://github.com/RanaAhmar/awesome-mcp-servers)** - The ultimate collection of Model Context Protocol implementations.
- **[System Design Cheatsheet](https://github.com/RanaAhmar/system-design-cheatsheet)** - Master complex architectures in minutes.
- **[Next.js SaaS Starter](https://github.com/RanaAhmar/nextjs-saas-starter)** - The fastest way to launch your next product.

### 🔗 Stay Connected
- **Website:** [stackaura.com](https://www.stackaura.com/)
- **Author:** [Ahmar Hussain](https://github.com/RanaAhmar)

---
