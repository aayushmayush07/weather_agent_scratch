# Weather Agent from Scratch

This project demonstrates how to build an intelligent weather agent **from scratch** without relying on frameworks like LangChain. The agent leverages OpenAI's GPT-3.5 model and a custom-designed toolset to answer weather-related queries in an iterative Thought-Action-Observation loop.

---

## Features

- **Custom Agent Architecture**: Built entirely from scratch using Python.
- **Dynamic Thought-Action-Observation Loop**: Mimics human-like reasoning, action, and observation to answer questions.
- **Weather Data Integration**: Uses Open-Meteo API to fetch real-time weather information.
- **Extensible Design**: Designed to easily integrate more tools or APIs if needed.

---

## How It Works

1. **Thought**: The agent reasons about the question asked.
2. **Action**: The agent performs an action, such as fetching weather data, and pauses.
3. **Observation**: The agent processes the results of the action and decides the next step.
4. **Answer**: The agent finally generates a response based on its observations.

This loop continues iteratively until the agent has enough information to provide a complete answer.

---

## Tools Used

- **OpenAI GPT-3.5**: For natural language understanding and reasoning.
- **Open-Meteo API**: For fetching real-time weather data.
- **Python Libraries**:
  - `os`: To fetch environment variables.
  - `re`: For regex-based text processing.
  - `requests`: For making API calls.

---

## Prerequisites

1. **Python 3.8+**
2. **Virtual Environment (Recommended)**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # For Linux/macOS
   venv\Scripts\activate     # For Windows
