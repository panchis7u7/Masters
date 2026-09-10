### Overview

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

### Data
API json documentation for Cisco SD-WAN vManage component will be stored in the vector database for fast lookups: `https://172.18.121.104:13001/apidocs/vmanageapi.json`

### Project Setup
1. Create a python virtual environment and install the dependencies.
```sh
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

2. Make jupyter notebook reference the the ipykernel from the virtual environment.