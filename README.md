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

## Example
### Input
`web=Website('https://www.vit.ac.in/')`

### Output
The assistant will provide a concise summary in markdown, such as:

### Summary of https://www.vit.ac.in/

The webpage is the official website of Vellore Institute of Technology (VIT). It contains information about:
- Admissions and academic programs.
- Research and development activities.
- Events and news updates related to the institute.
- Links to student portals, faculty details, and online resources.

Key announcements:
- Admission deadlines for various programs.
- Updates on recent achievements and ongoing events.

## Troubleshooting
### Git Push Issues
If you encounter errors like:
`! [rejected] main -> main (fetch first)`

Run the following commands to synchronize your local and remote repositories:
`git pull origin main --rebase`
`git push -u origin main`

## Contributing
Contributions are welcome! Feel free to open issues or create pull requests for improvements.

## License
This project is licensed under the [MIT License](LICENSE).

## Acknowledgments
- **VIT Official Website**: For providing a demonstration use case.
- **Ollama LLM**: For language model support.
