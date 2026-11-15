# Python Doubt Solver - AI Question-Answering Chatbot

A simple command-line chatbot built with **LangChain** and **Google Gemini** that answers Python questions.

## Features
- Gemini language model connected through LangChain
- Prompt template (system role + user question)
- User question as input, AI-generated answer as output
- API key stored safely in a `.env` file
- Basic error handling (missing key, empty input, API/network errors)

## Project Structure
```
langchain_project/
├── app.py
├── .env
├── requirements.txt
└── README.md
```

## Setup (VS Code)
1. Open the `langchain_project` folder in VS Code.
2. Open the terminal (`Ctrl + ~`) and create a virtual environment:
   ```
   python -m venv venv
   ```
3. Activate it:
   - Windows: `venv\Scripts\activate`
   - Mac/Linux: `source venv/bin/activate`
4. Install libraries:
   ```
   pip install -r requirements.txt
   ```
5. Get a free API key from https://aistudio.google.com/app/apikey and paste it in `.env`:
   ```
   GOOGLE_API_KEY=your_real_key_here
   ```
6. Run the chatbot:
   ```
   python app.py
   ```

## Sample Test Questions
1. What is the difference between a list and a tuple?
2. How does a for loop work in Python?
3. What is a lambda function? Give an example.
4. Explain what `*args` and `**kwargs` mean.
5. How do I handle exceptions using try and except?

## Technologies
Python, LangChain, Google Gemini, python-dotenv

## Note
Never share or upload your `.env` file (add it to `.gitignore` if using Git).
