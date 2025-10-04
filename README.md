# PranavGupta-langsmith-MAT496
This is my MAT496 project
Pranav Gupta
2410110241


# Module 1



## Lesson 1: Tracing basics

This project demonstrates how **LangSmith tracing** provides observability for a RAG application by capturing execution details.  

- **Projects** → containers for multiple traces  
- **Traces** → full end-to-end execution of a request  
- **Runs** → individual units of work (e.g., retrieval, generation)  
- `@traceable` → decorator to auto-log inputs, outputs, errors, and metadata  

### Key Updates  
- Swapped OpenAI calls with **Claude**  
- Replaced embeddings with **HuggingFace**  
- Adjusted notebook to better test RAG workflow  

Tracing enables debugging by replaying the exact sequence of operations and inspecting results in the **LangSmith web UI**.  

## Lesson 2: Types of Runs  

This lesson explains the different **types of runs** in an LLM application and how they appear in a trace.  

- **Chain Runs** → represent the overall workflow  
- **Tool Runs** → represent external calls/tools within the chain  
- **LLM Runs** → represent direct calls to the language model  

### Why It Matters  
- Helps distinguish workflow steps for **debugging** and **optimization**  
- Run hierarchy pinpoints **errors or bottlenecks**  
- Traces can be **filtered by run type** for focused inspection  

## Lesson 3: Alternative Tracing methods

This lesson explores different ways to trace LLM applications beyond LangChain’s built-in tools.  

- **LangChain Built-in Tracing** → simple and integrated  
- **OpenTelemetry** → open-source, framework-agnostic  
- **Phoenix** → visual interface for exploring traces and complex chains  

### Key Approaches  
1. **Context Manager (`with trace()`)** → custom control over inputs/outputs  
2. **Wrapper (`wrap_anthropic`)** → automatic tracing by wrapping the client (modified from `wrap_openai`)  
3. **RunTree API** → full manual control for building custom frameworks  

I modified the notebook/code to replace OpenAI with **Anthropic (Claude)** for compatibility.  
