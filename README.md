# my-python-langchain-crash-course
Basically practicing what i learned from langchain certification course (by langchain) and few extra features.

## How to start project

### create virtual environment first
- In case you haven't installed yet, install uv package manager.

- Then initiliaze your project for uv.
```uv init```

- Create virtual environment
```uv venv```

- Activate virtual environment
```.\.venv\Scripts\activate```

### Install all dependent packages
- fill requirement.txt file with all required packages for project
```
langchain
langchain_community
langchain-openai
langchain-groq
python-dotenv
langchain-google-genai
ipykernel
```
- run command
```uv add -r requirements.txt```

### create environment file
- create .env file inside venv
- create respective api keys for google-ai, groq, openai
- provide those keys into .env
- ensure your .gitignore file must has .env so that github can't see your sensitive secrets when you push code


