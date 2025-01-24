# Weather Agent from Scratch

This project demonstrates how to build an intelligent weather agent **from scratch** without relying on frameworks like LangChain. The agent leverages OpenAI's GPT-3.5 model and a custom-designed toolset to answer weather-related queries in an iterative Thought-Action-Observation loop.

---

## Features

- **Custom Agent Architecture**: Built entirely from scratch using Python.
- **Dynamic Thought-Action-Observation Loop**: Mimics human-like reasoning, action, and observation to answer questions.
- **Weather Data Integration**: Uses Open-Meteo API to fetch real-time weather information.
- **Extensible Design**: Designed to easily integrate more tools or APIs if needed.

---

## Tools Used

- **OpenAI GPT-3.5**: For natural language understanding and reasoning.
- **Open-Meteo API**: For fetching real-time weather data.
- **Python Libraries**:
  - `os`: To fetch environment variables.
  - `re`: For regex-based text processing.
  - `requests`: For making API calls.
  - `dotenv`: For loading environment variables from a `.env` file.

---

## Prerequisites

1. **Python 3.8+**

2. **Clone the Repository**:
    ```bash
    git clone git@github.com:aayushmayush07/weather_agent_scratch.git
    cd weather_agent_scratch
    ```

3. **Create and Activate a Virtual Environment**:
    ```bash
    python -m venv venv
    ```

    - **For Linux/macOS**:
        ```bash
        source venv/bin/activate
        ```
    - **For Windows**:
        ```bash
        venv\Scripts\activate
        ```

4. **Install Dependencies**:
    Install the required libraries using the provided `requirements.txt` file:
    ```bash
    pip install -r requirements.txt
    ```

5. **Set Up the `.env` File**:
    Create a `.env` file in the root directory of the project and add the following:
    ```env
    OPENAI_API_KEY=your_openai_api_key
    ```
    Replace `your_openai_api_key` with your actual OpenAI API key.

6. **Load Environment Variables**:
    The `.env` file will automatically be loaded using the `dotenv` library.

---

## Usage

### 1. Run the Agent

Start the agent by executing the main Python script:
```bash
python my_agent_scratch.py
