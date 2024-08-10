# AI Chatbot Using LLaMA or Your API of Choice

This project is an AI chatbot that can be powered by any API of your choice, such as the LLaMA API, Groq API, or others. The chatbot is designed to provide detailed and helpful responses based on user input, simulating a knowledgeable and descriptive conversation partner. The project also includes a custom HTML frontend to interact with the Gradio backend.

## Features

- **AI Chatbot**: Provides responses to user inputs with helpful and descriptive answers.
- **Customizable Backend**: You can integrate the chatbot with any API of your choice.
- **Custom Frontend**: A clean, modern chat interface built with HTML and CSS that connects seamlessly with the Gradio backend.
- **Keyboard and Button Support**: Allows users to send messages either by pressing "Enter" or clicking the "Send" button.

## Prerequisites

Before using this project, you need:

1. **Python Environment**: Ensure you have Python installed.
2. **API Key**: For the API of your choice (e.g., LLaMA API, Groq API, etc.).
3. **Gradio Backend**: A Gradio-based backend running with the API of your choice.

## Installation

### 1. Set Up the Backend

1. **Clone or Download the Backend Repository**:
    ```bash
    git clone https://github.com/your-username/your-repository.git
    cd your-repository
    ```

2. **Install the Required Python Packages**:
    ```bash
    pip install gradio
    pip install [API-Specific-Library]  # Replace with the library needed for your chosen API
    ```

3. **Configure Your API Key**:
    - Replace `YOUR_API_KEY` in the backend Python script with your actual API key.

4. **Run the Backend**:
    - Run the backend script using your preferred Python environment. Ensure `share=True` is enabled in Gradio to get a public URL.

    Example:
    ```python
    iface.launch(share=True, inline=False, inbrowser=False)
    ```

    Note down the public URL provided by Gradio.

### 2. Set Up the Frontend

1. **Edit the HTML File**:
    - Open the `index.html` file in a text editor.
    - Locate the line with `const gradioUrl = "https://your-gradio-url.gradio.app";` and replace the URL with the one provided by your Gradio backend.

2. **Host the HTML File**:
    - You can open the `index.html` file directly in your browser, or host it on any web server of your choice.

3. **Test the Chatbot**:
    - Once the HTML file is hosted and opened in a browser, you can interact with the chatbot. Type your message in the input box and either press "Enter" or click "Send" to get a response.
