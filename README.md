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

You need to get your **Groq API Key** and **RapidAPI Key**.  You may store the keys in your environment variables using:
```bash
export GROQ_API_KEY="your_groq_api_key"
export RAPIDAPI_KEY="your_rapidapi_key"
```
Alternatively, you may clone the repo and replace the keys in the code.

### API Call

The agent fetches blood glucose data from `human.p.rapidapi.com`. The API accepts a date parameter to return the corresponding glucose level.

## Usage

Once you have the setup ready, you can run the AI health agent. The agent will:

- Retrieve blood glucose data for a specified date.
- Analyze the data and provide health advice based on the glucose level.

### Example Query

You can input queries like:

- "What is my blood glucose level today?"

## Customization

You can modify the roles and backstories of the agents or adjust the tasks for more personalized use cases. For instance, you can add tasks to provide additional health insights or track more health metrics.

