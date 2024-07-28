# Context-Aware-Chatbot-with-Proactive-Assistance-and-Multi-Language-Support
This project aims to enhance user interactions with a context-aware chatbot that can handle complex queries, provide proactive assistance, and offer multi-language support with localization.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Overview
The project integrates three main components:
1. **Context-Aware Chatbot**: Uses advanced NLP techniques to maintain context over multiple interactions, enabling more coherent and relevant responses.
2. **Proactive Assistance**: Tracks user activity and proactively offers assistance, such as sending reminders for upcoming deadlines or suggesting relevant services.
3. **Multi-Language Support with Localization**: Provides responses in multiple languages based on the user’s geographical location, ensuring inclusivity and better communication.

## Features
### Context-Aware Chatbot
- Leverages a pre-trained transformer model (DialoGPT) to maintain conversation context.
- Offers an API endpoint for users to interact with the chatbot.

### Proactive Assistance
- Tracks user activities and sends proactive reminders or suggestions based on user behavior.
- Runs a background thread to monitor activities and send timely notifications.

### Multi-Language Support with Localization
- Uses a simple dictionary-based translation for demonstration purposes.
- Provides an API endpoint for localized responses based on user preferences.

## Installation
To install and run the project, follow these steps:

### Prerequisites
- Python 3.7+
- Google Colab account
- Required Python libraries: `flask`, `flask-ngrok`, `transformers`, `torch`

### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/sid1018/context-aware-chatbot.git
   cd context-aware-chatbot
   ```

2. Open the notebook in Google Colab:
   - `Context_Aware_Chatbot.ipynb`

3. Install the required libraries within the notebook:
   ```python
   !pip install flask-ngrok flask transformers
   ```

4. Run each cell in the notebook to execute the code.

## Usage
### Chat Interaction
1. Load the `Context_Aware_Chatbot.ipynb` notebook in Google Colab.
2. Run the cells to start the Flask API.
3. Use the `/chat` endpoint to send POST requests with `user_id` and `message` to interact with the chatbot.

### Proactive Assistance
1. Track user activities and receive proactive reminders or suggestions.
2. The proactive assistance feature runs automatically in the background.

### Localized Responses
1. Use the `/localized_response` endpoint to send GET requests with `user_id` and `key` to get translated responses.

## Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes. Ensure that your code adheres to the project's coding standards and includes relevant tests.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
