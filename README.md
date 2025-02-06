# Advanced RAG combines both GraphRAG and native vector-based RAG

In this repo, I am trying to build an advanced RAG which can decide on what knowledge base to use for grounding its answers. The solution is implemented with LangChain, Neo4j, Milvus and Bedrock. In particular, I am using two LLMs (Claude 3 sonnet and Mistral 7*8b) for performing different tasks. The idea is to use adavanced model, like Claude 3 sonnet, for buidling Graph database and generating Cypher query to run on the graph databse, while using less advanced model to conduct all the other tasks. For example, text generation for QA chain.

