RAG systems use vector databases to retrieve relevant information before generating a response.

Although multiple technologies exist, it is unclear which offers the best balance between:

 + Retrieval accuracy
 + Latency
 + Resource consumption
 + Final quality of generated responses

When used as external memory for AI agents.
For this investigation, we will compare the following databases:

 + [FAISS](https://github.com/facebookresearch/faiss)
 + [PGVector](https://github.com/pgvector/pgvector)
 + [Neo4j](https://neo4j.com/solutions/neo4j-vector-search/)
  + [Redis](https://redis.com/solutions/vector-database/)