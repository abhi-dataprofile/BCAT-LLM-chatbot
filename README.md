# LLM Chatbot for Buffalo Center for Arts and Technology (BCAT)

## Objective:
To develop a conversational chatbot using Snowflake tables, OpenAI API, and Streamlit that retrieves data from Snowflake based on user queries and showcases the results interactively. The goal is to enhance information accessibility for stakeholders by allowing natural language queries to generate actionable insights.

## Project Description:
This project leverages a **Large Language Model (LLM)** to act as an interface between stakeholders and the data stored in Snowflake. The chatbot is built using **Streamlit** for user interaction, **OpenAI's API** for natural language understanding and query generation, and **Snowflake** for secure data storage and retrieval.

The workflow involves:
1. Receiving user prompts (queries).
2. Applying prompt engineering with predefined rules to ensure data security and accuracy.
3. Generating optimized SQL queries based on the input and knowledge base.
4. Fetching data from Snowflake tables and displaying the results in an easy-to-read format.

## Workflow Overview:
1. **Knowledge Base as Prompts:**
   - Used structured prompts to guide the LLM in query generation.
   - Established key rules for query optimization and limiting access to sensitive information.

2. **Data Source and Query Generation:**
   - Provided the LLM with metadata about Snowflake tables (e.g., columns, data types).
   - Incorporated stakeholder-specific query formats to tailor responses to business needs.
   
3. **Query Execution and Display:**
   - Sent the generated SQL query to Snowflake for execution.
   - Retrieved and displayed results within the Streamlit application in tabular or visual formats (e.g., graphs, charts).
   
## Key Features:
- **Dynamic SQL Generation:** Automatically generates SQL queries based on stakeholder input.
- **Secure Data Access:** Follows rules for accessing and querying specific Snowflake tables.
- **User-Friendly Interface:** Built with **Streamlit** for intuitive interaction and visualization.
- **Real-Time Data Retrieval:** Retrieves up-to-date information directly from Snowflake.

## Skills and Technologies Used:
- **Natural Language Processing:** OpenAI API
- **Data Storage and Querying:** Snowflake
- **Web Application Framework:** Streamlit
- **Prompt Engineering:** Custom rule-based prompts for LLM
- **Version Control:** GitHub ([Repository Link](https://github.com/abhi-dataprofile/BCAT-LLM-chatbot/tree/main/Tech%20Bulls))

## System Architecture:
```plaintext
1. User Input (Stakeholder's Query) → 2. LLM (OpenAI API) → 3. Knowledge Base Rules →  
4. SQL Query Generation → 5. Snowflake Table Access → 6. Data Retrieved → 7. Display on Streamlit App
