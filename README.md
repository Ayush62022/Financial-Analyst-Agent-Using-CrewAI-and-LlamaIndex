# Financial-Analyst-Agent-Using-CrewAI-and-LlamaIndex


 
#### This project is designed to analyze an annual report and generate insightful content using advanced AI tools. The process involves:

Data Retrieval: Downloading a specific annual report in PDF format.
Data Parsing: Extracting and processing text from the PDF.
Embedding and Indexing: Converting the text into a format suitable for efficient querying.
Query Engine Setup: Creating a system to perform detailed searches and queries on the indexed data.
Task Automation: Using AI agents to perform tasks such as research and content creation based on the data.
Results Generation: Producing a comprehensive analysis and engaging blog post from the processed data.
 
### Installation of Dependencies:

Purpose: To ensure all required libraries and tools are available for processing and analyzing the data.
Details: Install Python packages such as llama-index, crewai, and others that provide functionalities like embedding generation, LLM operations, and file reading.
### Setup LLM with Groq:

Purpose: To configure the language model (LLM) that will be used for querying and analysis.
Details: Sign up at Groq for API keys and initialize the LLM with these keys. Test the model to ensure it's functioning as expected by making a test request.
Setup Chat Model for Crew AI:

Purpose: To establish a chat-based LLM that will handle specific interactions and queries.
Details: Configure ChatOpenAI with Groq’s API settings to enable chat-based functionalities and responses.
### Download Data:

Purpose: To acquire the source document (Infosys Annual Report 2022-23) for analysis.
Details: Use wget to download the PDF from a given URL.
Parse PDF Content:

Purpose: To convert the PDF into a format that can be analyzed.
Details: Use SimpleDirectoryReader to read and extract text and metadata from the downloaded PDF.
### Setup Embedding Model:

Purpose: To transform the document text into vector embeddings suitable for similarity searches.
Details: Initialize the embedding model (BAAI/bge-small-en-v1.5) which converts text into numerical vectors that capture semantic meaning.
Build Index:

Purpose: To organize the document data for efficient querying.
Details: Create a VectorStoreIndex from the parsed document using the embedding model. This index allows for fast and relevant search results.
### Build Query Engine:

Purpose: To enable searching and querying within the indexed data.
Details: Develop a query engine that interacts with the index to retrieve relevant information based on user queries.
### Instantiate Query Tool:

Purpose: To define how queries will be structured and what data will be used.
Details: Set up a LlamaIndexTool for querying the Infosys report, specifying its purpose and schema to guide the analysis.
### Instantiate Researcher and Writer Agents:

Purpose: To automate the tasks of research and content creation.
Details: Create two AI agents:
Researcher: Performs a detailed analysis of how Infosys uses AI based on the annual report.
Writer: Creates a blog post about Infosys’s use of AI, making it engaging and informative.
### Define Tasks:

Purpose: To outline specific goals for the AI agents to achieve.
Details:
Task 1: Research the use of AI by Infosys and produce a comprehensive analysis.
Task 2: Write a blog post based on the research, highlighting key insights in a casual style.
### Instantiate and Run Crew:

Purpose: To execute the defined tasks using the AI agents.
Details: Create a Crew instance with the defined agents and tasks, and run the workflow to complete the analysis and content creation.
Output:

Purpose: To present the results of the analysis and content generation.
Details: The final output includes a detailed analysis report and a blog post about Infosys’s use of AI, based on the processed data.
## Working Points
### Install Dependencies:

Install necessary Python packages (llama-index, crewai, etc.) to support various functionalities of the project.
### Setup LLM with Groq:

Sign up for Groq and obtain an API key.
Initialize the Groq LLM and test its functionality by making a sample request.
### Setup Chat Model for Crew AI:

Define and configure a chat-based LLM using ChatOpenAI with Groq’s API settings.
### Download Data:

Use wget to fetch the Infosys Annual Report in PDF format.
Parse PDF Content:

Utilize SimpleDirectoryReader to extract text and metadata from the downloaded PDF.
### Setup Embedding Model:

Initialize the embedding model to convert text into vector embeddings.
### Build Index:

Create a VectorStoreIndex from the embedded text for efficient querying.
### Build Query Engine:

Develop a query engine to interact with the index and retrieve relevant information.
### Instantiate Query Tool:

Set up a LlamaIndexTool to define the querying process and schema.
### Instantiate Researcher and Writer Agents:

Create AI agents for research and content writing tasks.
### Define Tasks:

Outline specific tasks for the AI agents, including research and blog post creation.
### Instantiate and Run Crew:

Create a Crew instance and execute the tasks to generate results.
Output:

 





