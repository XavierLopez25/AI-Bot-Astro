# Astro Docs Bot - Wiki Assistant

## Description
This repository contains the source code for a Wiki Assistant Bot designed to provide in-depth answers related to any specified subject by utilizing the Astro (JavaScript Framework) documentation. It leverages state-of-the-art natural language processing and document search technologies to deliver precise responses sourced from the official Astro documentation.

## Key Features
- **Document Extraction:** Utilizes a `DocsLoader` designed specifically for the Astro documentation site, processing and extracting key information for easy access.
- **Indexing and Search:** Employs `PineconeVectorStore` for robust document indexing and quick retrieval, powered by embeddings from OpenAI.
- **Dynamic Interaction:** Features a responsive user interface using Streamlit, enabling real-time user interactions and dynamic responses.
- **Chat History:** Keeps a record of all user queries and responses to refine future interactions and contextual understanding.

## Technologies Used
This project is crafted using Python alongside several other specialized libraries and platforms:
- **Astro** for web documentation handling.
- **LangChain** for language processing and chatbot logic.
- **OpenAI** for powerful embeddings and AI model functionalities.
- **Pinecone** for efficient vector index management.
- **Streamlit** for building the interactive web interface.
- **Beautiful Soup** and **Requests** for web scraping and data management.

## Installation
Follow these steps to set up the Astro Docs Bot on your local machine:

1. **Clone the Repository:**
```bash
  git clone https://github.com/XavierLopez25/AI-Bot-Astro.git
```

2. **Install Dependencies:**
Navigate to your project directory and install required Python libraries:
```bash
  pip install -r requirements.txt
```

3. **Create an Index in Pinecone:**
Configure a new index on Pinecone to manage the embeddings used by the bot. Visit Pinecone to set up the index.

4. **Set Up Environment Variables:**
Create a `.env` file in the root directory and include the following variables:
```bash
  OPENAI_API_KEY=your_openai_api_key_here
  PINECONE_API_KEY=your_pinecone_api_key_here
  INDEX_NAME=your_index_name_here
```

5. **Run Ingestion Script:**
Load the Astro documentation into your Pinecone index:
```bash
python ingestion.py
```

6. **Start the Streamlit Server:**
Launch the user interface through Streamlit:
```bash
streamlit run main.py
```

## Usage
Once the setup is complete, open the Streamlit interface and start querying about the Astro documentation. The bot processes your questions and retrieves answers directly from the indexed content.

## Sample Questions for Astro Docs Assistant Bot
Feel free to explore the capabilities of the Astro Docs Assistant Bot with queries like:
- What is Astro?
- How do I create a new project in Astro?
- What are the main features of Astro?
- How does Astro handle static rendering?
- What are the best practices for optimizing an Astro site for SEO?

## Demonstration
**Video Link:** https://youtu.be/DZ3LGCmuAXo
