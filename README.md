# ChatBot-using-APIKey
Here's a brief overview of what the script does:

Installs necessary packages (langchain, openai, and chromadb) using pip.
Sets the OpenAI API key.
Defines a CSVLoader to load data from a CSV file (client_data_bcg.csv assumed to be located in the "Downloads" directory).
Creates a vector index using VectorstoreIndexCreator.
Constructs a question-answering chain using RetrievalQA, specifying OpenAI's language model (LLM) for text generation, a custom chain type ("stuff" in this case), and a retriever based on the created vector index.
Provides a query ("give me small info of the data") to the chatbot chain.
Prints the response received from the chatbot.
