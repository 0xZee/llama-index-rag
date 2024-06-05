# llama-index-rag Notebook
- LLM Inference via `GROQ API`
- LLM Model : `llama3-8b`
- Embedding Model : HuggingFace Embedding `BAAI/bge-small-en-v1.5`
- chat Engin : `Condense question`


# Chat Engine - Condense Question Mode
Condense question is a simple chat mode built on top of a query engine over your data.

For each chat interaction:

1. First generate a standalone question from conversation context and the last message.
2. Query the query engine with the condensed question for a response.

This approach is simple and works well for questions directly related to the knowledge base. However, since it always queries the knowledge base, it can have difficulty answering meta questions like "what did I ask you before?"
