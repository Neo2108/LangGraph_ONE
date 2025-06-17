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

WRITE:
- State Schema
- Create required nodes
- Add nodes
- Add edges
- Compile graph

Nodes: Functions that take state and return updated state
Graph: Add nodes
Edge: Add edges or conditional edges to connect multiple nodes

----------------------------------------------------------------------------------------

Workflows -> Predefined code paths with LLMs and tools
Agents -> LLMs dynamically direct their own processes

Agent: LLM Call through query, LLM directs action to a specific TOOL and then outputs
Prompt Chaining: In -> Out
Parallelizatoin: Multiple LLMs called and multiple outputs given
Orchestrator-Worker: Input goes to orchestrator, orchestrator breaks up tasks between workers and then sends to a synthesizer
Evaluator-optimizer: Input goes to Generator LLM and then that data goes to an Evaluator LLM, then output is given
Routing: Input given to one LLM and output to two different LLMs

----------------------------------------------------------------------------------------

PROMPT CHAINING: 
- Input goes to LLM Call 1
- LLM Call 1 outputs to Gate
- IF FAILS: Exit, IF GOOD: Pass to LLM Call 2
- Outputs to LLM Call 3
- Finally outputs result


