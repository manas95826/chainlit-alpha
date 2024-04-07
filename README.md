# Chainlit - Alpha

## Overview
Chainlit - Alpha Chatbot is a conversational AI powered by the LangChain framework and Hugging Face models. It serves as a general chatbot capable of answering questions related to enterprises. The chatbot is built to be deployed as a Docker container, ensuring easy deployment and scalability.

## Features
- General chatbot functionality
- Enterprise-related question answering
- Dockerized deployment for portability and scalability

## Requirements
- Python 3.9
- Docker

## Installation
1. Clone the repository:
    ```
    git clone https://github.com/manas95826/chainlit-alpha.git
    cd chainlit-alpha
    ```

2. Install dependencies:
    ```
    pip install -r requirements.txt
    ```

## Usage
1. Set up your Hugging Face API token by creating a `config.py` file and defining `HUGGINGFACEHUB_API_TOKEN`.

2. Build the Docker image:
    ```
    docker build -t chainlit-alpha .
    ```

3. Run the Docker container:
    ```
    docker run -d -p 7860:7860 chainlit-alpha
    ```

## Configuration
- The `template` variable in `app.py` defines the chatbot's behavior and responses. Modify this to customize the chatbot's behavior.
- You can adjust the `max_length` and `temperature` parameters in the `HuggingFaceEndpoint` instantiation to control the chatbot's response length and creativity, respectively.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Create a new Pull Request

## License
This project is licensed under the [MIT License](LICENSE).
