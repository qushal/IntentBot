# IntentBot
# Chatbot Assistant

A simple chatbot assistant built with PyTorch and NLTK that can be trained on custom intents and responds to user input.

## Features

- Trainable on custom intents from a JSON file
- Uses bag-of-words and lemmatization for text processing
- Neural network model with PyTorch
- Easily extendable with custom functions for specific intents

## Requirements

- Python 3.7+
- PyTorch
- NLTK
- NumPy

Install dependencies with:
```sh
pip install torch nltk numpy
```

## Setup

1. Download NLTK data (uncomment these lines in `main.py` if running for the first time):
    ```python
    nltk.download('punkt')
    nltk.download('wordnet')
    nltk.download('omw-1.4')
    ```
2. Prepare your `intents.json` file with your intents, patterns, and responses.
3. Run the script to train the model:
    ```sh
    python main.py
    ```
   This will create `chatbot_model.pth` and `dimensions.json`.

## Usage

- After training, the chatbot will prompt you for input.
- Type your message and get a response.
- Type `/quit` to exit.

## Customization

- Add new intents and responses in `intents.json`.
- Extend functionality by mapping intents to custom Python functions in `ChatBotAssistant`.

## License

MIT License
