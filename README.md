# AI_Voice_Assistant

## Project Goal

The goal of this project is to create a user-friendly application that allows users to interact with the Gemini LLM through voice commands.

## Technical Stack
* Speech Recognition: SpeechRecognition library to capture user voice input.
* Large Language Model (LLM): Google Gemini LLM (accessed using the Google Generative AI library) for text generation and conversation flow.
* Text-to-speech: gtts library to convert generated text responses to audio.
* Web Framework: Streamlit for building a user interface for interaction.

## Functionality

Voice Input:

* The application uses the SpeechRecognition library to listen for user voice commands.
* The recorded audio is then converted to text using Google Speech Recognition service.

Text Processing:

* The captured user query is sent to the Gemini LLM through the Google Generative AI library.

LLM Response Generation:

* The Gemini LLM processes the user query and generates a text response.

Text-to-Speech Output:

* The generated text response is converted to audio using the gtts library.

User Interface:

* Streamlit is used to create a user interface for the application.
* The interface displays the user query, the LLM response text, and allows playback of the generated speech.


## Running the Application

1: Prerequisites:
* Python 3.x
* pip (Python package manager)
* Install required libraries:
  
            Bash
            pip install speech_recognition google-generativeai dotenv gtts streamlit

2: Set Up Google API Key:
* Create a Google Cloud Project and enable the Google Generative AI API.
* Obtain an API Key and store it securely using the dotenv library.
* You can find instructions on obtaining an API Key here: https://cloud.google.com/ai/generative-ai
3: Run the application:
* Open a terminal or command prompt and navigate to the project directory.
* Run the script:
  
            Bash
            python main.py

4: Interact with the Assistant:
* Open http://localhost:8501/ in your web browser.
* Click the "Ask me anything" button.
* Speak your question or request.
* The application will convert your speech to text, send it to the Gemini LLM, and display the generated response along with an audio playback option.
This is a basic description of the AI Voice Assistant. You can further enhance the project by adding features like:

## Multilingual Support: 
*  Enhance the application to support multiple languages.
## Contextual Awareness: 
* Allow the LLM to maintain conversation context for more natural interactions.
## Customizable Responses: 
* Allow users to configure response formats or integrate with other services.
