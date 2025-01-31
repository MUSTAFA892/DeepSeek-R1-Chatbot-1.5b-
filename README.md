# DeepSeek R1 Chatbot: AI Coding Assistant

DeepSeek R1 is a powerful AI-powered coding assistant designed to help developers with their coding tasks. Whether you need help debugging, writing code, designing solutions, or adding documentation, DeepSeek R1 can assist you in real-time with minimal input. Built with **Ollama** and **LangChain**, DeepSeek R1 is optimized for Python code and provides interactive and intelligent suggestions.

---

## Features

- **Python Expert**: Understands and assists with Python code, including debugging and code design.
- **Debugging Assistant**: Helps find and resolve bugs in your code using strategic print statements.
- **Code Documentation**: Provides detailed documentation for your code and functions.
- **Solution Design**: Helps design efficient solutions for coding problems and projects.
  
---

## Installation and Setup

### Prerequisites

To use DeepSeek R1, you must have the following installed:

- **Python 3.x** or later
- **Streamlit** (for the web interface)
- **LangChain** (for the underlying language model integration)
- **Ollama** (for the model engine)

You can install Streamlit and LangChain via pip:

```bash
pip install streamlit
pip install langchain
```

Ensure you have Ollama set up locally, as it will be used as the backend engine for processing requests. You can download Ollama from the official website: [Ollama](https://ollama.ai/).

---

## How to Use

### Starting the Application

Once the setup is complete, you can start the chatbot application by running the following command in your terminal:

```bash
streamlit run app.py
```

This will launch a web interface where you can interact with DeepSeek R1.

### Chat Interface

The interface consists of the following sections:

1. **Sidebar**: 
   - **Model Selection**: Choose between two model variants, `deepseek-r1:1.5b` and `deepseek-r1:3b`. You can pick the model based on the required response complexity or processing power.
   - **Model Capabilities**: Overview of what the chatbot can do (e.g., Python assistance, debugging, documentation).

2. **Chat Display Area**: 
   - Messages from the user and AI are displayed here. The AI responds to your queries based on the conversation history.

3. **Chat Input**: 
   - Type your coding question in the input box, and DeepSeek R1 will generate a response.

---

## Customization

DeepSeek R1 is customizable to suit specific needs or preferences. You can modify the following:

1. **Model Configuration**: 
   - The `selected_model` option in the sidebar lets you choose the model variant for your task.

2. **System Prompt**:
   - The `system_prompt` defines the behavior of the AI. The template provided encourages concise and correct responses, focusing on strategic debugging and solution design.

3. **Styling**:
   - Custom CSS is included to ensure the interface is clean, modern, and easy to use.

---

## How It Works

- **Input Handling**: 
   - When you type a coding question in the input field, DeepSeek R1 sends the query to the AI model.
  
- **AI Response Generation**: 
   - The model generates a response based on the conversation history, which includes previous user inputs and AI replies.
  
- **Model Engine**:
   - DeepSeek R1 uses **ChatOllama** to invoke the appropriate AI model and generate responses. The `StrOutputParser` ensures that the model's output is clean and formatted for user presentation.

---

## Example Usage

1. **Debugging Code**: 
   - **User**: "I'm getting an IndexError in my code. Can you help me debug it?"
   - **AI**: "Sure! Let's start by checking the list index you're using. Here's a potential fix with a print statement for debugging."

2. **Code Explanation**: 
   - **User**: "Can you explain how the `map()` function works in Python?"
   - **AI**: "The `map()` function applies a given function to each item of an iterable (like a list) and returns a map object. Here's an example..."

3. **Solution Design**: 
   - **User**: "How would you design a program to find the factorial of a number?"
   - **AI**: "A simple way to calculate the factorial of a number is by using recursion. Here's a basic implementation..."

---

## Contributing

We welcome contributions to improve the chatbot! If you find any issues or have feature requests, feel free to create an issue or submit a pull request. 

### Steps to Contribute:

1. Fork the repository.
2. Create a new branch for your changes.
3. Make your changes and commit them.
4. Submit a pull request with a description of your changes.

---

## License

DeepSeek R1 is open-source and available under the MIT License.

---

## Acknowledgments

- **Ollama** for providing the AI engine.
- **LangChain** for enabling easy integration with language models.
- **Streamlit** for creating a simple yet powerful UI for chat-based applications.

---



