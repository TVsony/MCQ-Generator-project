# MCQ Generator and Evaluator

This repository contains a sophisticated Python application for generating and evaluating Multiple Choice Questions (MCQs) tailored for educational purposes.
The project leverages OpenAI's GPT-3.5 Turbo model via LangChain to produce quizzes based on input text and provides comprehensive feedback to refine the quiz
questions for better alignment with the target audience.

---

## 🚀 Features

1. **Automated Quiz Generation**:
   - Dynamically generates MCQs based on input text.
   - Supports customization for the number of questions, subject matter, and tone.

2. **Quiz Evaluation and Refinement**:
   - Analyzes the cognitive complexity and quality of generated questions.
   - Suggests and applies changes to ensure quizzes align with students' abilities.

3. **Modular Design**:
   - Easy integration of components for text processing, MCQ generation, and evaluation.
   - Supports chaining of tasks for end-to-end quiz development.

4. **Customizable Templates**:
   - Templates designed for precise control over question tone, format, and complexity analysis.

5. **Seamless API Integration**:
   - Environment-variable-based API key management using `dotenv`.

---

## 🛠️ Technologies Used

- **Programming Language**: Python 3.9+
- **LLM Framework**: [LangChain](https://www.langchain.com/)
- **OpenAI API**: GPT-3.5 Turbo for natural language understanding.
- **Data Handling**: Pandas for dataset processing.
- **Environment Management**: Python `dotenv` for secure API key storage.
- **Logging**: Custom logging for debug and information tracking.

---

## 📚 Prerequisites

Before running the application, ensure you have the following:

1. Python 3.9 or later installed.
2. An active OpenAI API key.
3. Required Python dependencies installed via `requirements.txt`.

---

## 🔧 Installation
1 Create and activate a virtual environment:
conda create -p venv python==3.10 -y

2 Install dependencies: 
pip install -r requirements.txt

3 Set up your .env file:
Create a .env file in the root directory.
Add your OpenAI API key 
OPENAI_API_KEY='Your OPENAI API KEY '

## 🚀 Usage
1. Generate and Evaluate MCQs
Run the main script with required inputs:
Streamlit run mcqgenerator.py

## 2. Inputs
The application uses the following inputs:

text: Source text for generating MCQs.
number: Number of MCQs to generate.
subject: Subject matter for tailoring the quiz.
tone: Desired tone for questions (e.g., formal, casual).

## 3. Outputs
Quiz: A JSON-formatted quiz based on the input text.
Review: Analysis and refined suggestions for the generated quiz.

## 🧩 Project Structure
mcq-generator/
├── src/
│   ├── mcqgenerator/
│   │   ├── utils.py       # Utility functions for text/file handling.
│   │   ├── logger.py      # Custom logging setup.
│   │   ├── __init__.py    # Package initialization.
│   ├── main.py            # Entry point for the application.
├── tests/                 # Unit tests for the project.
├── .env                   # Environment variables (not included in the repo).
├── .gitignore             # Files and directories to ignore in version control.
├── requirements.txt       # Required Python packages.
└── README.md              # Project documentation.

# 🧪 Example 

Text: "Newton's laws of motion are three physical laws that together laid the foundation for classical mechanics. ..."
Number: 5
Subject: Physics
Tone: Formal

## 🛡️ Error Handling
The application logs errors and debug information in a logs/ directory.
Common issues, such as missing API keys or input text, are handled with user-friendly error messages.

## 🤝 Contributions
Contributions are welcome! Feel free to open issues, submit pull requests, or suggest enhancements.

Fork the repository.
Create a feature branch.
Commit your changes.
Open a pull request.

## 🙏 Gratitude
A heartfelt thank you to the LangChain team for their exceptional framework, which made this project possible.
Deep appreciation to OpenAI for providing cutting-edge language models that power the heart of this application.
A special thanks to the Krish Naik and Sunny Savita invaluable resources and inspiration.
