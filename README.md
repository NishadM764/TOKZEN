#  TOKZEN — AI Prompt & Token Optimizer
<img width="668" height="518" alt="tokzen-logo" src="https://github.com/user-attachments/assets/58ed0149-6433-4b1b-8a16-9ab29d73474f" />

## Overview

TOKZEN is a Python-based application designed to analyze and optimize prompts used with AI models.

Long prompts can contain unnecessary words, repeated instructions, and redundant information. TOKZEN helps users analyze their prompts, identify areas for improvement, and generate shorter alternatives.

By combining rule-based text processing with AI-powered semantic compression, TOKZEN aims to reduce token usage while preserving the original prompt's important meaning and intent.

## Features

- **Token Analysis** — Analyze the token, word, and character counts of a prompt.
- **Prompt Quality Analysis** — Evaluate prompt clarity, relevance, specificity, structure, and redundancy.
- **Rule-Based Compression** — Remove unnecessary wording using text-processing rules.
- **Semantic Compression** — Generate concise prompt alternatives using AI-powered processing.
- **Token Reduction Analysis** — Compare the original and optimized prompts to understand how much the token count has changed.
- **Interactive Interface** — Explore prompt analysis and compression through a Streamlit web application.

## How It Works

TOKZEN follows a simple workflow to analyze and optimize prompts.
### Step-by-step workflow

1. **Input:** The user enters a prompt.
2. **Token Analysis:** The application measures the prompt's token, word, and character counts.
3. **Quality Analysis:** The prompt is evaluated for clarity, relevance, specificity, structure, and redundancy.
4. **Compression:** The application applies rule-based or AI-powered compression.
5. **Re-analysis:** The optimized prompt is analyzed again.
6. **Comparison:** The original and optimized token counts are compared.

## Tech Stack

| Technology      | Purpose                                |
| --------------- | -------------------------------------- |
| Python          | Core application logic                 |
| Streamlit       | Interactive web interface              |
| Tiktoken        | Token counting                         |
| Text Processing | Rule-based prompt compression          |
| LLM API         | AI-powered semantic compression        |
| Python Modules  | Modular analysis and compression logic |

*The technologies listed above should match the packages and services used in your actual implementation.*

## Getting Started

Follow these instructions to run TOKZEN on your local machine.

### Prerequisites

- Python 3.10 or later
- pip package manager
- Git
- An API key, if required by your semantic compression implementation

### 1. Clone the repository

```bash
git clone https://github.com/NishadM764/ai-token-optimizer.git
cd ai-token-optimizer
```

### 2. Create a virtual environment

```bash
python3 -m venv .venv
```

### 3. Activate the virtual environment

**macOS / Linux**

```bash
source .venv/bin/activate
```

**Windows**

```bash
.venv\Scripts\activate
```

### 4. Install dependencies

If your repository contains a `requirements.txt` file, run:

```bash
pip install -r requirements.txt
```

Otherwise, install the packages your application actually requires. For example:

```bash
pip install streamlit tiktoken
```

Install any additional dependencies required by your AI provider or compression modules.

### 5. Configure your API key

If semantic compression uses an external AI service, configure the required API key using an environment variable or an appropriate local secrets configuration.

Never upload API keys, passwords, or other secrets to GitHub.

### 6. Run the application

If `app.py` is your Streamlit entry point, run:

```bash
streamlit run app.py
```

If your main Python file has a different name, replace `app.py` with the correct filename.

## Token Reduction Analysis

TOKZEN compares the token counts of the original prompt and the optimized prompt.

| Metric               | Description                                                |
| -------------------- | ---------------------------------------------------------- |
| Original Tokens      | Number of tokens in the original prompt                    |
| Optimized Tokens     | Number of tokens in the compressed prompt                  |
| Tokens Saved         | Difference between the original and optimized token counts |
| Reduction Percentage | Percentage decrease in token count                         |

### Calculation

**Tokens Saved**

```text
Original Tokens - Optimized Tokens
```

**Token Reduction Percentage**

```text
((Original Tokens - Optimized Tokens) / Original Tokens) × 100
```

For example, suppose a prompt contains 200 tokens before compression and 150 tokens after compression.

- Original tokens: 200
- Optimized tokens: 150
- Tokens saved: 50
- Token reduction: 25%

These values are illustrative. Actual results depend on the prompt and the compression method used.

If the original prompt contains zero tokens, the reduction percentage should not be calculated.

## Project Structure

The project may be organized as follows. Update the filenames to match your actual repository.

```text
ai-token-optimizer/
├── app.py
├── Token_Analysis.py
├── prompt_compression.py
├── semantic_compression.py
├── prompt_analysis.py
├── requirements.txt
├── tokzen-logo.png
└── README.md
```

### Main components

- **Application Interface:** Provides the interface for entering and analyzing prompts.
- **Token Analysis:** Calculates token, word, and character counts.
- **Prompt Analysis:** Evaluates the quality of the input prompt.
- **Rule-Based Compression:** Simplifies prompts using text-processing rules.
- **Semantic Compression:** Uses an AI model to generate concise alternatives.
- **README:** Documents the project, installation process, and features.

## Applications

TOKZEN can be useful for:

- Developers working with large language models.
- Students learning about prompt engineering.
- AI application builders looking to optimize prompts.
- Researchers experimenting with prompt compression.
- Users who want to compare original prompts with shorter alternatives.

## Future Improvements

Potential improvements include:

- Support for additional AI models and tokenizers.
- More advanced prompt compression strategies.
- Automated tests for compression quality.
- Benchmarks for semantic preservation.
- Exportable prompt analysis reports.
- Additional visualizations for comparing prompt characteristics.

## Limitations

- Compression results vary depending on the input prompt.
- Shorter prompts do not always produce better AI responses.
- Rule-based compression may remove wording that is important in some contexts.
- AI-powered compression depends on the selected model and its configuration.
- Token counts can differ between models because different tokenizers may be used.

Users should review the optimized prompt before using it in an important workflow to ensure that essential instructions and context remain intact.

## Author

**Nishad M**

GitHub: [@NishadM764](https://github.com/NishadM764)

Project repository: [AI Token Optimizer](https://github.com/NishadM764/ai-token-optimizer)

## Contributors

- **Nishad M** — Project development, core implementation, and integration.
- **Tharun Shiva R** — Collaborative development, feature contributions, testing, and project improvements.

We worked together to build TOKZEN, an AI-powered prompt optimizer designed to analyze prompts and reduce token usage while aiming to preserve their original meaning.

## License

This project does not specify a license yet. Add a `LICENSE` file if you intend to distribute the project as open-source software.

---

\<p align="center">   \<strong>TOKZEN\</strong>   \<br>   \<em>Compress More. Spend Less.\</em> \</p>

