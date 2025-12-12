
2025-12-09 13:22

Status: #Finished

Tags: [[AI]] [[agents]] 

# Langchain

- Langchain helps us create agents and apps powered by LLMs
- Use Langchain when you want to quickly create agents or autonomous apps
- Use LangGraph if you want a more advanced and deterministic and agentic workflow
- LangGraph is low-level. Langchain is high-level.
- Langchain is open-source orchestration framework for app development consisting of AI

- Langchain consists of:
	- LLM = any model
	- Prompts = Prompt template class for the model
	- Chains = Core workflow. Combines model with other components
	- Indexes
		- Doc Loader = 3rd party services to load/get data like google drive or drop box for example
		- VectorDB = Vector embeddings
		- Text Splitters = Split text into small semnticaly meaningful chunks
	- Memory = You can retain entire conversations as well as retain summary of the entire conversation
	- Agents = Uses the given model to reason as to "which actions to take"

### Components of Langchain:
1. Input processing
	1. Document loader
	2. Text splitter
	3. Documents
2. Embedding and Storage:
	1. Vectors
	2. Vector storage
3. Retrieval
	1. User Query
	2. Embedding models
	3. Query vector
	4. Retrievals (from vector storage which gets us relevant context)
4. Orchestration
	1. Agents
	2. Memory
5. Generation
	1. LLM
	2. AI response
	3. Tools
	4. Tool results

==1. INPUT PROCESSING = Converts text to structured documents==

==2. EMBEDDING AND STORAGE = Convert text into searchable vector representations==

==3. RETRIEVAL = Find relevant information based on user query==

==4. GENERATION = Uses AI models to create responses. Optionally with tools==

==5. ORCHESTRATION = Coordinate everything through agents and memory==



#### References
