# Flask_CRUD_App

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Initialize the database

Run this once before starting the app:

```bash
flask --app app shell
```

Then enter:

```python
from app import db

with app.app_context():
    db.create_all()
exit()
```

## Run the app

```bash
python app.py
```

Open [http://localhost:5001](http://localhost:5001) in your browser.
