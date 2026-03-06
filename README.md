AI Smart Health Supportizer using LangGraph
📌 Project Description
AI Smart Health Supportizer is a simple AI-based health assistant built using Python and LangGraph.
The system takes user symptoms as input and provides basic health advice by retrieving relevant health information and generating responses using an AI model.

This project demonstrates the use of AI agents, vector memory, and natural language processing to build an intelligent health support system.

⚠️ This system provides basic health suggestions only and does not replace professional medical advice.

🎯 Project Objectives

Build an AI health assistant

Analyze user health symptoms

Retrieve relevant health information

Generate AI-based health suggestions

Demonstrate LangGraph agent workflow

🧠 System Workflow
User Input
   ↓
LangGraph Agent
   ↓
Retrieve Context from Memory (FAISS)
   ↓
AI Model (GPT-2) generates response
   ↓
Health Advice Output
📁 Project Structure
AI-Smart-Health-Supportizer/
│
├── main.py
├── graph_builder.py
├── memory_store.py
├── utils.py
└── README.md
📄 File Description
main.py

This file runs the main application.

Functions:

Accepts user input

Sends the input to the AI agent

Displays the generated health advice

Example:

You: I have fever and cough
Health Assistant: Drink warm fluids and take rest.
graph_builder.py

This file creates the LangGraph workflow for the AI agent.

It contains:

State definition

Retrieve node

Generate node

Graph compilation

The workflow connects memory retrieval and AI response generation.

memory_store.py

This file manages the health knowledge memory.

It uses:

Sentence Transformers for text embeddings

FAISS vector database for similarity search

The system retrieves the most relevant health information based on user symptoms.

utils.py

This file contains helper functions used in the program.

Example:

print_separator() function to display a separator line in terminal output.

⚙️ Technologies Used

Python

LangGraph

Transformers (GPT-2)

LangChain

FAISS Vector Database

Sentence Transformers

📦 Installation

Install the required libraries:

pip install langgraph langchain langchain-community transformers sentence-transformers faiss-cpu
▶️ Running the Project

Run the following command:

python main.py
💬 Example Input
You: I have headache
💡 Example Output
Health Assistant:
Headache may be caused by dehydration.
Drink enough water and take rest.
🚀 Future Improvements

Add voice-based symptom input

Integrate real medical datasets

Develop a web interface using Streamlit

Connect with hospital APIs

📚 Learning Outcomes

Through this project we learned:

AI Agent workflow using LangGraph

Vector search using FAISS

Natural language generation using Transformers

Building AI-based health support systems using Python
