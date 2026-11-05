# Auto Tinder Bot

This Selenium script signs in to the configured TinDog demo app through its Facebark login flow, dismisses the onboarding prompts, and attempts to like 20 profiles.

## Requirements

- Python 3.8 or newer
- Google Chrome or Chromium
- Selenium and python-dotenv

Install the Python dependencies:

```bash
python -m pip install selenium python-dotenv
```

Selenium Manager can locate or download a compatible browser driver. You need a working Chrome or Chromium installation.

## Configuration

Create a `.env` file next to `main.py`:

```dotenv
FACEBARK_EMAIL=your-demo-account-email
FACEBARK_PASSWORD=your-demo-account-password
```

The credentials are read from this local file rather than stored in the script. Do not commit or share the `.env` file. Use only an account you are authorized to access and check the service's rules before automating interactions.

## Run

From this directory, run:

```bash
python main.py
```

The script opens Chrome, attempts up to 20 likes, and closes the browser when finished.
