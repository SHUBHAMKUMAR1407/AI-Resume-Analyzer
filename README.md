# AI-Resume-Analyzer

AI-Resume-Analyzer is a Streamlit-based academic project by **Shubham Kumar** from **Rajiv Gandhi Institute of Petroleum Technology (RGIPT)**.

It helps users review and improve resumes using document parsing, rule-based analysis, AI-assisted feedback, resume building, job-role suggestions, and analytics.

## Features

- Upload and analyse PDF or DOCX resumes
- ATS-oriented score and keyword feedback
- Role-based skills and resume recommendations
- AI-assisted resume analysis using configured providers
- Resume builder with downloadable document output
- Resume analytics dashboard and feedback collection
- Job search and company suggestions

## Tech stack

- Python and Streamlit
- SQLite for local data storage
- PyPDF/PDFPlumber and python-docx for document extraction
- Google Gemini/OpenRouter integrations through environment variables
- Plotly, pandas, spaCy and scikit-learn for analysis and visualisation

## Run locally

```bash
python -m venv venv
```

Windows:

```bash
venv\Scripts\activate
```

macOS/Linux:

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
python -m spacy download en_core_web_sm
```

Create `utils/.env` from `utils/.env.example` and add the API keys required for AI analysis. Never commit real keys.

Start the application:

```bash
streamlit run app.py
```

## Project structure

```text
AI-Resume-Analyzer/
|-- app.py                   # Streamlit application
|-- config/                  # Roles, courses and database configuration
|-- dashboard/               # Analytics dashboard
|-- feedback/                # Feedback collection
|-- jobs/                    # Job search and suggestions
|-- style/                   # Application styling
|-- utils/                   # Parsing, analysis, AI and resume builder logic
|-- assets/                  # Application assets
|-- requirements.txt
`-- CREDITS.md
```

## Academic project

**Student:** Shubham Kumar
**Institute:** Rajiv Gandhi Institute of Petroleum Technology (RGIPT)
**Project:** AI-Resume-Analyzer

## Attribution

This repository contains adapted components from an MIT-licensed open-source resume analyzer. The original copyright notice is retained in `LICENSE`, and the source attribution is documented in [CREDITS.md](CREDITS.md).

## License

See [LICENSE](LICENSE) and [CREDITS.md](CREDITS.md).
