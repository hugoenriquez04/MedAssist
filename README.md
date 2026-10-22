# MedAssist

MedAssist is an AI-powered clinical data assistant designed to help healthcare professionals query and analyze patient information through a web interface. The application combines a Flask backend, a JavaScript frontend, a SQLite database, and a language model to provide natural-language access to clinical information.

## Team Members

- Hugo Enríquez Jiménez
- Luis Alarcón Arroyo
- Verónica Rodríguez Brome
- Ana García Temboury

## Features

- Natural-language interaction with a clinical data assistant.
- Patient information lookup through a web interface.
- Clinical data queries generated with the help of a language model.
- Visualization of query results as tables and charts.
- Patient conversation history and PDF report generation.
- Support for general medical questions and patient-specific queries.

## Project Structure

```text
MedAssist/
├── Backend/
│   ├── backend.py
│   ├── requirements.txt
│   ├── .env.example
│   └── README.md
├── Frontend/
│   ├── index.html
│   ├── script.js
│   ├── style.css
│   └── README.md
├── .gitignore
└── README.md
```

## Requirements

- Python 3.9 or later
- A valid API key for the configured language-model service
- A modern web browser

## Installation

1. Clone the repository:

   ```bash
   git clone <repository-url>
   cd MedAssist
   ```

2. Create and activate a virtual environment:

   ```bash
   python -m venv .venv
   ```

   On Windows:

   ```powershell
   .\.venv\Scripts\Activate.ps1
   ```

   On macOS or Linux:

   ```bash
   source .venv/bin/activate
   ```

3. Install the backend dependencies:

   ```bash
   pip install -r Backend/requirements.txt
   ```

4. Create `Backend/.env` from `Backend/.env.example` and provide your own API key:

   ```env
   API_KEY=your_api_key_here
   ```

   Never commit `.env` or any API key to the repository.

## Running the Application

1. Place an authorized local demonstration database at `Backend/database.db`.
   The database is intentionally not included in this repository because it contains clinical data.

2. Start the backend:

   ```powershell
   python Backend/backend.py
   ```

3. Open `Frontend/index.html` in a web browser.

The backend runs locally at `http://127.0.0.1:5000/`.

## Data and Privacy

Clinical datasets, local databases, generated reports, and environment files are excluded from this repository. They must not be committed unless their publication has been explicitly authorized and they contain no personal or confidential information.

The application is intended for demonstration and educational purposes only. It must not be used for real medical diagnosis, treatment decisions, or clinical care.


