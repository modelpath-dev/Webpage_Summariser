# Webpage Summarizer

A Python-based application that fetches and analyzes the contents of a webpage, providing concise summaries of the page's content. It intelligently ignores navigation-related text and extracts key information, including news and announcements, if available.

## Features
- Fetches webpage content using the given URL.
- Parses HTML and extracts meaningful text, excluding scripts, styles, images, and input elements.
- Generates short summaries of the webpage content using an AI language model.
- Summaries are structured in markdown format for easy readability.

## Requirements
- Python 3.8+
- `requests` library
- `beautifulsoup4` library
- Ollama LLM API (running locally at `http://localhost:11434`)
- OpenAI Python SDK

## Installation
1. Clone the repository:
   `git clone https://github.com/modelpath-dev/Webpage_Summariser.git`
   `cd Webpage_Summariser`
2. Set up a Python virtual environment:
   `python -m venv llms`
   `source llms/bin/activate # On Windows: llms\Scripts\activate`
3. Install dependencies:
   `pip install -r requirements.txt`
4. Ensure the Ollama LLM API is running locally.

## Usage
1. Start the application by running the `app.ipynb` file in your preferred Jupyter Notebook environment.
2. Update the URL in the `web=Website('<url>')` line to the desired webpage you wish to summarize.
3. Run the code to generate a concise summary of the webpage's content.


## Contributing
Contributions are welcome! Feel free to open issues or create pull requests for improvements.


