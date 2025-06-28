# 🧠 MemoryAgent – A Memory-Augmented LLM Agent Using Letta and MemGPT Architecture
> **Reason. Recall. Respond.**  
> Intelligent agent with persistent memory, dynamic reasoning, and tool-calling capabilities.

---

## 📌 Overview

**MemoryAgent** is an intelligent, stateful LLM-based agent system engineered using the open-source **Letta framework**, and inspired by the **MemGPT architecture** (*"Towards LLMs as Operating Systems"*). It introduces a two-tiered memory hierarchy and agentic execution loop, enabling persistent knowledge management, dynamic reasoning, and tool-augmented responses across interactions.

---

## 🔁 Agent Loop

The agent operates on a modular reasoning cycle:

Observe → Think → Act → Update Memory


This enables contextual processing and long-term memory integration for intelligent, stateful behavior.

---

## 🔧 Key Features

### ✅ Tiered Memory Management
- **Core Memory**: Injected into the LLM’s context window for real-time use  
- **Archival Memory**: Stored externally, retrieved via semantic search  
- **Memory Blocks**: JSON-based structured units tagged for efficient lookup and storage

### 🔍 Semantic Retrieval
- Integrates **FAISS** for vector similarity search  
- Uses OpenAI’s `text-embedding-ada-002` to embed and retrieve relevant archival memory based on context

### ⚙️ Tool Invocation
- Dynamically calls external tools such as:
  - Python functions (e.g., calculators, converters)
  - APIs or services
- Driven by reasoning-based function call architecture

### 🔁 Self-Editing & Summarization
- Summarizes long memory blocks when needed  
- Automatically updates or prunes outdated facts using schema-based pipelines

### 🧑‍🤝‍🧑 Multi-Agent Collaboration
- Enables communication between multiple agents  
- Agents can share memory blocks or delegate tasks via message passing and shared state

---

## 🚀 Use Cases

- Personal Assistant with long-term memory  
- Academic Tutor that remembers student progress  
- Knowledge Manager for researchers or teams  
- Planner Bot that remembers tasks, events, and goals  
- Autonomous Agent with contextual awareness

---

## 🧰 Tech Stack

| Component | Tech |
|----------|------|
| Programming Language | Python |
| Framework | [Letta](https://github.com/letta-ai/letta) |
| LLM API | OpenAI GPT-4 + `text-embedding-ada-002` |
| Vector Search | FAISS |
| Memory Format | JSON-based core & archival blocks |
| Architecture | Async Agent Loops + Reasoning Modules |

---



