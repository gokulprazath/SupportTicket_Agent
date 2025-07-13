# SupportTicket_Agent
Building a simple SupportTicket_Agent using langgraph.
Steps to replicate 
1) Create a copy of the colab.
2) Generate api_key of ur wish and Include it in environment.
3) Run it in a flow.

## Description:

This notebook demonstrates how to build a support agent using `pydantic-ai` that interacts with a SQLite database to manage support tickets. The key steps covered are:

1.  **Installation**: Installing the necessary libraries, including `pydantic-ai`, `crewai`, `openai`, and `pydantic-ai-slim[groq]`.
2.  **Model Definition**: Defining the language model to be used by the agent. In this case, a Groq model is configured.
3.  **Agent Definition and Run**: Defining the `SupportAgent` with its dependencies, output type, and system prompt. This section also shows how to run the agent with a specific prompt and dependencies.
4.  **Database Operations (Manual)**:
    *   Creating a SQLite database and a `tickets` table.
    *   Inserting sample ticket data into the table.
    *   Displaying the data currently in the table.
    *   Removing all data from the table (optional).
5.  **Agent Tools**: Defining the tools that the `SupportAgent` can use to interact with the database:
    *   `insert_ticket`: To add new tickets.
    *   `extract_details`: To retrieve details of existing tickets.
    *   `update_details`: To modify details of existing tickets.
