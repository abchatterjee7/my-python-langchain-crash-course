# my-python-langchain-crash-course
# Python LangChain Crash Course

A hands-on collection of exercises and experiments based on the LangChain certification course, with a few additional features. This project is for learning LangChain and trying its integrations with different language-model providers.

## Prerequisites

- Python
- [uv](https://docs.astral.sh/uv/)
- API keys for whichever providers you plan to use

## Getting started

Run the commands below from the project directory.

### 1. Initialize the project if needed

If the project does not already have a `pyproject.toml`, initialize it with:

```powershell
uv init
```

### 2. Create and activate a virtual environment

```powershell
uv venv
.\.venv\Scripts\Activate.ps1
```

For Command Prompt, activate it with:

```cmd
.\.venv\Scripts\activate.bat
```

### 3. Install dependencies

If the project contains a `requirements.txt`, install its packages with:

```powershell
uv pip install -r requirements.txt
```

The requirements file should contain the packages needed by the project. For example:

```text
langchain
langchain_community
langchain-openai
langchain-groq
langchain-google-genai
python-dotenv
ipykernel
```

Adjust this list to match the packages actually used by the exercises.

## Configure API keys

Create a `.env` file in the **project root** (not inside `.venv`) and add the keys required by your code. For example:

```text
OPENAI_API_KEY=your-openai-key
GROQ_API_KEY=your-groq-key
GOOGLE_API_KEY=your-google-ai-key
```

Use the environment-variable names expected by the relevant scripts. You only need keys for the providers you use.

Ensure `.env` is listed in `.gitignore`. Never commit or share real API keys.

## Run the exercises

Browse the project’s Python files and notebooks, then run the exercise you want to try. To run a Python file:

```powershell
python path\to\your_file.py
```

Open notebooks in VS Code or Jupyter. The `ipykernel` dependency allows the virtual environment to be used as a notebook kernel.

Check each exercise for provider-specific setup, required environment variables, and usage instructions.

## Troubleshooting

- **A package cannot be imported:** Confirm the virtual environment is active and install the dependencies.
- **An API request fails:** Verify that the required key is set in `.env`, its variable name matches the code, and the key is valid.
- **PowerShell blocks environment activation:** Use the Command Prompt activation command above, or follow your organization’s guidance for PowerShell execution policy.


