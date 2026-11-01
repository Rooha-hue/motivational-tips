# motivational-tips
# 🔥 Daily Motivation

A small Streamlit app that gives you a personalized motivational message,
three tiny action steps and an affirmation, powered by Google Gemini Flash.

## Features

- **Personal boost** - choose your mood, what you're working on and a tone
  (Gentle friend, Coach, Stoic mentor, Playful)
- **Quick quote** - a built-in quote library that works without an API key
- **History** for the current session, plus a download button for any message

## Run locally

```bash
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install -r requirements.txt
export GEMINI_API_KEY="your-key"   # free key: https://aistudio.google.com
streamlit run app.py
```

Alternatively create `.streamlit/secrets.toml` (do not commit it):

```toml
GEMINI_API_KEY = "your-key"
```

or paste the key into the sidebar.

## Changing the model

Default is `gemini-2.5-flash`. Change it in the sidebar or set `GEMINI_MODEL`.
Current model names: https://ai.google.dev/gemini-api/docs/models

## Deploy on Streamlit Community Cloud

1. Push this repo to GitHub.
2. Go to https://share.streamlit.io, click **Create app**, pick the repo, branch `main`, file `app.py`.
3. In **Advanced settings → Secrets** add `GEMINI_API_KEY = "your-key"`.
4. Click **Deploy**.

## Note

This app offers encouragement, not professional or medical help.
