# 🤖 Research Agent

An **AI-powered research agent** that analyzes developer tools, frameworks, and platforms using **web crawling, LLM-based reasoning, and structured data extraction**.  
Built with **LangGraph**, **OpenAI GPT**, and **Firecrawl**, this system autonomously discovers, analyzes, and compares technologies to assist developers in making better tech choices.

---

## 🚀 Project Overview
**Research Agent** automates the process of discovering and evaluating developer-oriented products — from APIs to SDKs and cloud platforms.  
It uses multi-step reasoning to:
1. 🔍 Search for relevant tools and companies.
2. 🧠 Extract structured insights such as pricing, tech stack, and API availability.
3. 💬 Generate concise, data-informed recommendations for developers.

---

## 🧩 Core Components

| Component | Description |
|------------|--------------|
| `simple-agent.py` | Basic CLI version of the agent using Firecrawl MCP tools. |
| `advanced-agent.py` | Full workflow-driven agent integrating all analysis modules. |
| `src/models.py` | Defines structured Pydantic models for company and research data. |
| `src/prompts.py` | Contains specialized prompt templates for extraction, analysis, and recommendations. |
| `src/firecrawl.py` | Wrapper around the Firecrawl API for web search and scraping. |
| `src/workflow.py` | Implements the multi-step reasoning workflow using LangGraph. |

---

## ⚙️ Workflow
1. **Extract Tools** → Finds relevant tools and libraries from online sources.  
2. **Research** → Scrapes official pages and retrieves technical content.  
3. **Analyze** → Performs structured LLM-based extraction of pricing, API, stack, etc.  
4. **Recommend** → Generates a short, actionable summary comparing tools.

---

## 🧠 Example Use
```bash
Example Input

🔍 Developer Tools Query: best API management platforms

Example Output

📊 Results for: best API management platforms
1. 🏢 Postman
   🌐 Website: https://www.postman.com
   💰 Pricing: Freemium
   💻 Language Support: Python, JavaScript, Go
   🔌 API: ✅ Available
   📝 Description: API collaboration platform for developers.

Developer Recommendations:
Postman offers a balance between usability and enterprise features, making it ideal for small-to-medium teams.
```
## 🛠 Tech Stack

LangChain + LangGraph – workflow orchestration

OpenAI GPT-4o-mini – reasoning & structured LLM outputs

Firecrawl – intelligent web crawling and content scraping

Pydantic – data validation and serialization


## 📦 Installation
#### 1️⃣ Clone the repository
git clone https://github.com/<your-username>/research-agent.git
cd research-agent

#### 2️⃣ Create the environment using uv
```
uv venv
```
#### 3️⃣ Activate the environment
- on Windows
```
.venv\Scripts\activate
```
- on macOS/Linux
```
source .venv/bin/activate
```
#### 4️⃣ Install dependencies from pyproject.toml
```
uv sync
```
Add your API keys in a .env file:

OPENAI_API_KEY=your_openai_key
FIRECRAWL_API_KEY=your_firecrawl_key
---

