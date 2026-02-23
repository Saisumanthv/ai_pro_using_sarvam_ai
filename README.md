# Multi Model AI Project

A Streamlit-based web application that integrates **Sarvam AI** to provide Text-to-Speech conversion and AI-powered conversational responses with audio output — all in one place.

---

## Features

- **Text to Speech** — Convert any text input into natural-sounding speech using Sarvam AI's `bulbul:v3` TTS model with the `ratan` speaker voice.
- **Ask AI** — Submit a query to Sarvam AI's `sarvam-m` chat model and receive both a text response and its spoken audio version.
- **Personalized experience** — Enter your name to have your messages displayed with your name in the chat.
- **Sidebar navigation** — Clean option menu for switching between app sections.

---

## Tech Stack

- [Streamlit](https://streamlit.io/) — Frontend UI framework
- [Sarvam AI](https://www.sarvam.ai/) — Text-to-Speech & LLM APIs
- [streamlit-option-menu](https://github.com/victoryhb/streamlit-option-menu) — Sidebar navigation
- [python-dotenv](https://pypi.org/project/python-dotenv/) — Environment variable management

---

## Getting Started

### Prerequisites

- Python 3.8+
- A [Sarvam AI](https://www.sarvam.ai/) account and API key

### Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/multi_model_ai_project.git
cd multi_model_ai_project
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Set up your API key. You can do this in one of two ways:

   **Option A — `.env` file (local development):**
   ```
   SARVAM_API_KEY=your_api_key_here
   ```

   **Option B — Streamlit secrets (deployment):**  
   Create `.streamlit/secrets.toml`:
   ```toml
   SARVAM_API_KEY = "your_api_key_here"
   ```

### Running the App

```bash
streamlit run app.py
```

---

## Usage

1. Open the app in your browser (usually at `http://localhost:8501`).
2. Optionally enter your name in the sidebar.
3. Use **Text to Speech** to convert any text to audio, or use **Ask AI** to submit a question and get both a written and spoken response.

---

## Project Structure

```
multi_model_ai_project/
├── app.py                  # Main Streamlit application
├── .env                    # Local environment variables (not committed)
├── .streamlit/
│   └── secrets.toml        # Streamlit secrets for deployment
├── requirements.txt        # Python dependencies
└── README.md
```

---

## Requirements

Add the following to your `requirements.txt`:

```
streamlit
requests
sarvamai
streamlit-option-menu
python-dotenv
```

---

## License

This project is open source. Feel free to fork and build on it.
