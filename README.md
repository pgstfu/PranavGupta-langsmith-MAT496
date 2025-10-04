# PranavGupta-langsmith-MAT496
This is my MAT496 project
Pranav Gupta
2410110241

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
