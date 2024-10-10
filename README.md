# AI-Based-Chatbot-for-Emotional-Support-in-Anxiety-and-Depression

## Overview
This project focuses on the development of an AI-based chatbot designed to provide emotional support to individuals experiencing anxiety and depression. By leveraging advanced Natural Language Processing (NLP) techniques, the chatbot is capable of understanding user inputs and offering appropriate responses to help users manage their mental health.

The chatbot was developed using two main model architectures: Long Short-Term Memory (LSTM) and Gated Recurrent Unit (GRU). These models were trained on mental health-related conversations and evaluated based on key performance metrics such as accuracy, precision, recall, and F1-score.

## Features
- **Emotional Support**: Provides conversational support for users struggling with anxiety and depression.
- **NLP Models**: Implements LSTM and GRU for classifying user intents.
- **Predefined Intents**: The chatbot is trained on a variety of conversational intents (e.g., greetings, expressions of sadness, stress, anxiety).
- **Multiple Models**: Users can choose between LSTM or GRU-based chatbots for interaction.
- **Context Handling**: Supports maintaining context across multiple interactions.

## Project Structure
```bash
/AI-Chatbot-Emotional-Support
├── /src                          # Source code for chatbot logic
│   ├── chatbot.py                # Main chatbot implementation
├── /notebooks                    # Jupyter notebooks used in development
│   ├── app.ipynb                 # Notebook for chatbot implementation
│   ├── Development...ipynb       # Full project development notebook
├── /models                       # Pretrained chatbot models
│   ├── chatbot_model_GRU.keras   # GRU-based chatbot model
│   ├── chatbot_model_LSTM.keras  # LSTM-based chatbot model
├── /data                         # Data and resources
│   ├── intents.json              # Primary intent dataset
│   ├── words.pkl                 # Processed words for model input
│   ├── feedback.json             # Feedback data
├── README.md                     # Project documentation
├── requirements.txt              # Python package dependencies
└── .gitignore                    # Files to ignore in version control
```

## Installation

### Clone the repository:
```bash
git clone https://github.com/BalaElangovan/AI-Based-Chatbot-for-Emotional-Support-in-Anxiety-and-Depression.git
```

### Install dependencies:
```bash
pip install -r requirements.txt
```

### Download models:

Ensure you download the pre-trained models (chatbot_model_LSTM.keras, chatbot_model_GRU.keras) located in the /models directory. These models are required for the chatbot to function.

## Usage
### Running the Chatbot
### To interact with the chatbot:

1. Open any of the provided Jupyter notebooks (e.g., app.ipynb) to explore the chatbot's functionality.

2. Load either the LSTM or GRU model for processing user inputs:

```bash
model = load_model('models/chatbot_model_GRU.keras')
```

3. Enter your query, and the chatbot will respond with appropriate emotional support messages:

```bash
response = chatbot_response('I am feeling sad today.')
print(response)
```

## Available Intents
The chatbot can understand various conversational intents such as greetings, goodbyes, expressions of sadness, stress, or anxiety. You can find all available intents in the intents.json file.

## Model Comparison
This project compares the effectiveness of two NLP models (LSTM and GRU). The GRU model was found to perform slightly better in terms of generalization and computational efficiency based on key metrics (accuracy, F1-score).

## Future Improvements
- Expanding the dataset with more diverse conversational patterns.
- Enhancing the chatbot’s capability to detect complex emotional states.
- Integrating additional features like sentiment analysis or real-time interaction.

## Ethical Considerations
While this chatbot aims to provide basic emotional support, it is not intended as a replacement for professional mental health services. Users experiencing severe distress should seek help from licensed professionals.




