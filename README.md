# Simple Notes Web App

A simple web application where users can sign up, log in, write notes, and delete notes. This app is built using Flask, a lightweight Python web framework.

## Features

- User authentication (sign up and log in).
- Add new notes.
- View all your notes.
- Delete notes.

## Installation Guide

### Prerequisites

- Python 3.7 or later installed on your system.
- `pip` (Python package manager) installed.

### Steps

1. **Clone the Repository**

   ```bash
   git clone <repository_url>
   cd <repository_folder>
   ```

2. **Set Up a Virtual Environment** (optional but recommended)

   - On Windows:
     ```bash
     python -m venv venv
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     python3 -m venv venv
     source venv/bin/activate
     ```

3. **Install Dependencies**
   Install the required Python packages using the `requirements.txt` file:

   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up the Database**
   Initialize the SQLite database:

   ```bash
   flask db init
   flask db migrate -m "Initial migration."
   flask db upgrade
   ```

5. **Run the Application**
   Start the Flask development server:
   ```bash
   flask run
   ```
   The app will be available at `http://127.0.0.1:5000/`.

## Usage

1. Visit the home page.
2. Sign up for a new account.
3. Log in using your credentials.
4. Add, view, and delete notes.

## File Structure

```
project_folder/
|
├── app.py                  # Main Flask application file
├── models.py               # Database models
├── templates/              # HTML templates
│   ├── login.html          # Login page
│   ├── sign_up.html        # Sign-up page
│   ├── notes.html          # Notes page
├── static/                 # Static resources (CSS, JS, images)
├── requirements.txt        # Project dependencies
├── README.md               # Documentation file (this file)
└── .gitignore              # Git ignore file
```

## Requirements

All dependencies are listed in the `requirements.txt` file. To install them, run:

```bash
pip install -r requirements.txt
```

## Contributing

Contributions are welcome! If you'd like to contribute, please fork the repository and submit a pull request.

## License

This project is licensed under the Mouse License. See the `LICENSE` file for details.
