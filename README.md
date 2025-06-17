Node: No memory, no complex logic, linear processing only (LLM)

RAG Pipeline: External knowledge present, Context awareness present, Still linear flow present

Graph Architecture: Parallel processing enabled, conditional branching, state management, and there is a human-in-the-loop
multi-agent collaboration

----------------------------------------------------------------------------------------

Simple agents -> Single task
Conditional Agents -> Decision points, branching logic
Multi-agent Systems -> Collaborative, coordinated workflows

----------------------------------------------------------------------------------------

AGENT CONTROL Vs. RELIABILITY TRADE-OFF:
- Router Agent: High reliability, low control level
- Autonomous Agents: High control level, low reliability
- LangGraph: Provides a good balance between both

LangGraph: Framework for buliding stateful, multi-agent applications with LLMs, using graph-based workflows
-> State management, Graph Architecture, Multi-agent, Human-in-the-loop

----------------------------------------------------------------------------------------

Four Layers in the Ecosystem: Model Providers -> AI Framework Foundation -> Orchestration & Workflow -> Application Layer

Ex. (OpenAI/Gemini) -> (LangChain/LlamaIndex/Haystack) -> (LangGraph/CrewAI) -> (Customer support/Research Assistant)

----------------------------------------------------------------------------------------

CORE CONCEPTS of LangGraph:

Nodes: Functions that perform computation
Edges: Connections that route data between nodes
State: Shared data structure passed between nodes
Graph: The overall workflow structure

----------------------------------------------------------------------------------------

Nodes: Functions that take state and return updated state
Graph: Add nodes
Edge: Add edges or conditional edges to connect multiple nodes


