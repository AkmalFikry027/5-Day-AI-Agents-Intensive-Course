# 5-Day AI Agents Intensive — Kaggle Learn Guide

[![Course: 5-Day AI Agents Intensive](https://img.shields.io/badge/course-AI%20Agents%20Intensive-blue)](#)
[![Self-paced on Kaggle](https://img.shields.io/badge/platform-Kaggle-yellow)](#)
[![Status](https://img.shields.io/badge/status-available%20self--paced-success)](#)

Welcome to the 5-Day AI Agents Intensive — a practical, hands-on learn guide originally delivered live (Nov 10–14, 2025) by Google ML researchers and engineers and now published as a self-paced Kaggle Learn guide. This repository collects the curriculum, whitepapers, codelabs, notebooks, and deployment examples used in the program so you can learn how to design, build, evaluate, and productionize AI agents.

Table of Contents
- Overview
- Who this guide is for
- Learning outcomes
- Course structure (Day-by-day)
- Codelabs & hands-on notebooks
- Prerequisites & environment
- Quick start
- Best practices & production considerations
- Resources & reading
- Contributing
- License & contact

Overview
--------
AI agents are systems that can plan, act, and interact with tools and environments to achieve goals. This intensive blends conceptual deep dives with practical codelabs so you can move from prototypes to production-ready agentic systems. Throughout the guide you will explore models, tools, orchestration, memory, evaluation, observability, and deployment.

Who this guide is for
---------------------
- Developers and ML engineers building agentic systems
- Researchers interested in agent architectures and evaluation
- Platform and SRE engineers preparing to deploy agents at scale
- Product managers and technical leads wanting to understand agent trade-offs

Learning outcomes
-----------------
By the end of this guide you will be able to:
- Explain the core components of agent architectures: models, tools, orchestration, memory, and evaluation
- Build agents that use external tools and APIs (via MCP)
- Implement session-based context and long-term memory
- Instrument agents with logging, tracing, and metrics for observability
- Evaluate agent responses using automated and human-in-the-loop approaches
- Deploy agents to a production platform (Vertex AI Agent Engine) and design multi-agent systems with A2A

Course structure (Day-by-day)
-----------------------------
Day 1 — Introduction to Agents
- Foundations and taxonomy of agent capabilities
- Agent Ops: governance, reliability, security, identity, and constrained policies
- Codelabs:
  - Build your first AI agent (ADK + Gemini + Google Search)
  - Build a small multi-agent system (specialized agents + coordination patterns)

Day 2 — Agent Tools & MCP (Model Context Protocol)
- Designing external tools & safe tool usage patterns
- MCP architecture and interoperability considerations
- Codelabs:
  - Turn Python functions into agent-invokable tools
  - Implement long-running tool operations with human approval workflows

Day 3 — Context Engineering: Sessions & Memory
- Sessions (short-term conversational context) vs Memory (long-term persistence)
- Techniques for context management and retrieval-augmented flows
- Codelabs:
  - Make agents stateful using session context in ADK
  - Add persistent long-term memory across sessions

Day 4 — Agent Quality, Observability & Evaluation
- Observability pillars: Logs, Traces, Metrics
- Evaluation framework: LLM-as-a-Judge, automated scoring, HITL
- Codelabs:
  - Instrument agents (logs, traces, and metrics) and debug flows
  - Evaluate response quality and tool usage with automated and human judgments

Day 5 — Prototype to Production & A2A Protocol
- Production lifecycle: deployment, scaling, governance, monitoring
- Agent2Agent (A2A) Protocol for multi-agent collaboration
- Codelabs:
  - Build communicating multi-agent systems using A2A
  - Deploy an agent to Vertex AI Agent Engine (local → scalable service)

Codelabs & Notebooks
--------------------
Each day includes at least two codelabs/notebooks. Notebooks are designed to run on Kaggle or a local Python environment with minimal configuration. Example contents:
- day-01-agent-basics.ipynb — first agent using ADK + Gemini + Search
- day-01-multi-agent.ipynb — multi-agent patterns
- day-02-tools.ipynb — turning Python functions into agent tools
- day-03-sessions-memory.ipynb — session context handling
- day-03-long-term-memory.ipynb — persistent memory patterns
- day-04-observability.ipynb — logs, traces, metrics
- day-04-evaluation.ipynb — LLM-as-judge & HITL evaluation
- day-05-a2a.ipynb — Agent2Agent protocol demo
- day-05-deploy-vertex.ipynb — deploy to Vertex AI Agent Engine

Prerequisites & Environment
---------------------------
Recommended:
- Familiarity with Python and basic ML/LLM concepts
- Kaggle account (recommended for running notebooks with minimal setup)
- Google Cloud account to try Vertex AI Agent Engine deployment (optional for local work)
- (Optional) Access to Gemini or a compatible LLM for ADK examples

Quick start
-----------
1. Clone this repo.
2. Open the notebooks on Kaggle (recommended) or locally in Jupyter.
3. Follow Day 1 notebook to build and run your first agent.
4. Progress day-by-day through codelabs to learn tools, memory, evaluation, and deployment.

Best practices & production considerations
------------------------------------------
- Define strict tool contracts and fine-grained access control for external tools
- Implement observability from day one: logs, traces, and metrics
- Use evaluation pipelines (automated + human) to monitor quality continuously
- Plan for identity, constrained policies, and governance early (Agent Ops)
- Design agents as composable components to support A2A collaboration and scaling

Resources & reading
-------------------
- Course whitepapers (one per day) — included in /whitepapers
- ADK examples and API reference — included in /adk
- MCP (Model Context Protocol) spec and examples — included in /mcp
- A2A protocol examples — included in /a2a
- Kaggle Learn guide URL (self-paced): [insert Kaggle URL here]

Contributing
------------
We welcome contributions:
- Open an issue for bugs, feature requests, or content suggestions
- For notebooks and docs, submit a PR with clear description and testing steps
- Please follow the Code of Conduct and Contribution Guidelines in /docs


Acknowledgements
----------------
Course authored by Google ML researchers and engineers. Thank you to all contributors and the Kaggle community for helping make this resource available.
