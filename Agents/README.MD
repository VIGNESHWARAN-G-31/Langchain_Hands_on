# 🤖 Agents – LangChain Hands-on

This folder contains **practical experiments and notebooks** focused on **LangChain Agents** — AI systems that can decide which tool to use, in what order, and how to achieve a given goal.

---

## 📌 What Are Agents?
In LangChain, **Agents**:
- Use **LLMs** as the “brain”
- Decide **what actions to take**
- Choose the right **tools** for the job
- Receive observations and decide the **next step**
- Continue until the task is completed

Think of them as **smart managers** who coordinate between tools, data sources, and reasoning.

---

## 📂 Contents

### 1. `multiple_datasource_ragagent.ipynb`
- Demonstrates an agent using **multiple tools**.
- Tools include:
  - Wikipedia search tool
  - Math calculation tool
  - Custom retriever for Tamil Nadu data
- Shows how the agent chooses **the correct tool for each query** automatically.

---

### 2. `retriever_tool_agent`
- Focuses on **retriever-based agents**.
- Uses:
  - `create_retriever_tool()` from `langchain.tools.retriever`
  - Custom vector store (**FAISS**) for Tamil Nadu facts
- Agent responds with context-aware answers by fetching from the retriever.

---

### 3. `gemini_agent`
- Uses **Google Gemini** as the LLM for reasoning.
- Shows integration with:
  - `langchain-google-genai`
  - Gemini model selection (`gemini-pro`, `gemini-1.5-flash`, etc.)
- Demonstrates prompt handling & tool use within Gemini-powered agents.

---

### 4. `langchain_hub_agent`
- Pulls prompt templates from **LangChain Hub**.
- Example: Using a predefined “react” (Reasoning + Acting) prompt.
- Agent executes multi-step reasoning with hub-provided prompts.

---

### 5. `local_llm_agent`
- Uses **Gemma 3** local LLM for offline agent execution.
- Integrated with:
  - Local embeddings (`nomic-embed-text`)
  - FAISS for vector search
- Good for environments with no internet.

---

## 🛠 Skills Covered in This Folder
- Creating **custom tools** and integrating them with agents.
- Using `create_toll_calling_agent() ,AgentExecutor()`  and adapting for Gemini.
- **Retriever tools** for domain-specific data search.
- **LangChain Hub** for prebuilt prompts.
- Running agents with **API-based** and **local** LLMs.
- Managing rate limits and function naming rules for Gemini.
- Step-by-step **AgentExecutor** workflow.

---

## ✅ Outcomes
By going through the files here, you will:
- Understand **how agents decide which tool to use**.
- Build both **online** (API) and **offline** (local) AI agents.
- Learn to **connect LLMs with real-world data sources**.
- Gain confidence in **multi-tool AI workflows**.

---
