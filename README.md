A Retrieval-Augmented Generation (RAG) pipeline built with semantic chunking, leveraging LangChain, Hugging Face models, Pinecone vector database, and Groq LLM for accurate and 
context-aware responses.

Overview
This project implements a domain-specific chatbot that can respond to user queries by retrieving relevant information from a custom knowledge base and generating human-like responses using an LLM.

Key Highlights:

🔹 Semantic chunking for context-preserving document splitting

🔹 Embedding and similarity search with Pinecone

🔹 LLM inference via Groq for fast generation

🔹 LangChain used to chain components in a modular pipeline

🔹 Open-source models from Hugging Face

How to Run
1. Clone the Repository
git clone https://github.com/your-username/rag-chatbot.git
cd rag-chatbot

2. Install Dependencies
You can install required packages with:
pip install -r requirements.txt

3. Set Environment Variables
Create a .env file with the following keys:
PINECONE_API_KEY=your_key
PINECONE_ENVIRONMENT=your_environment
GROQ_API_KEY=your_key
HUGGINGFACE_API_TOKEN=your_token
You can also use %load_ext dotenv and %dotenv in the notebooks to load these.

4. Run Notebooks
Run the notebooks sequentially:

Open semantic_chunking.ipynb → Load & chunk your data.

Open rag_pipeline.ipynb → Generate embeddings, store in Pinecone, and query using Groq LLM.

🔎 Example Use Case
This setup is ideal for building a chatbot or knowledge assistant that:

Understands customer FAQs

Answers product-related queries

Leverages proprietary internal documentation

