# medallion-agent-NLP
Agentic RAG system that turns a messy system of record into a clean Bronze → Silver data model, with human-in-the-loop decision cards.

reads the documentation for a messy system of record (cryptic column names, coded values, docs that don’t always match the data), checks the claims against the actual data using read-only tools, and proposes a clean Silver-layer data model. When it’s unsure or finds a conflict, it sends a decision card to a human expert, and approved answers are stored as precedents so repeat questions decline over time.

We compare hybrid RAG vs. prompt-only QA, multi-agent vs. single-agent spec generation, and (optionally) fine-tuned DistilBERT vs. few-shot LLM conflict classification, using NHANES and the MIMIC-IV demo.

Team: Jack, Ryan, Skylar, Nikhil
