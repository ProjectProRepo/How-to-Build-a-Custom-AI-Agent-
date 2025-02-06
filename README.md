# Custom AI Health Agent
This project builds a custom AI health agent using **Groq's Llama3 model** and **CrewAI**. The agent fetches blood glucose levels from an external API and provides health insights and recommendations.

## Project Overview

This AI health agent utilizes:
- **LangChain-Groq**: To interact with the Llama3 model for inference.
- **CrewAI**: To orchestrate the tasks and handle agent interactions.
- **RapidAPI**: To fetch real-time blood glucose data using the `human.p.rapidapi.com` API.

The agents are designed as:
- **Data Fetcher Agent**: Responsible for fetching blood glucose data.
- **Analysis Agent**: Analyzes the fetched data and provides recommendations.

## Key Features
- **Real-time data retrieval**: Fetches blood glucose levels for a given date.
- **Health advice**: Provides personalized health insights and recommendations based on blood glucose levels.
- **Customizable agents**: You can modify the agents' roles and tasks for more specific use cases.

## Installation

To use the AI Health Agent, you need to install the required dependencies. You can install them using the following commands:

```bash
pip install pip --progress-bar off
pip install 'crewai[tools]'==0.28.8 --progress-bar off
pip install langchain-groq==0.1.3 --progress-bar off
```

## Setup

### API Keys:

You need to get your **Groq API Key** and **RapidAPI Key**.

Store the keys in your environment variables using:

```bash
export GROQ_API_KEY="your_groq_api_key"
export RAPIDAPI_KEY="your_rapidapi_key"
```

