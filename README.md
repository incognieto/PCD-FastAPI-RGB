# PCD-FastAPI-RGB

A simple web application built with **FastAPI** and **OpenCV** to upload digital images and display their RGB arrays. The app uses Bootstrap for responsive design and Jinja2 for templating.

## Features
- Upload images via a web interface.
- Display the uploaded image and its RGB channel arrays (Red, Green, Blue).
- Built with FastAPI, OpenCV, and Python.

## Prerequisites
- Python 3.8+
- Virtual environment (recommended)

## Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/PCD-FastAPI-RGB.git
   cd PCD-FastAPI-RGB
   ```
2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows
   ```
3. Install dependencies:
   ```bash
   pip install fastapi uvicorn jinja2 opencv-python-headless python-multipart sqlalchemy databases sqlite-utils
   ```
4. Create required directories:
   ```bash
   mkdir -p static/uploads templates
   ```

## Running the App
1. Run the FastAPI server:
   ```bash
   uvicorn main:app --reload
   ```
2. Open your browser and navigate to `http://127.0.0.1:8000`.

## Project Structure
```
├── main.py              # FastAPI backend
├── static/uploads       # Directory for uploaded images
├── templates            # HTML templates
│   ├── base.html
│   ├── home.html
│   └── display.html
└── README.md
```

## Usage
- Upload an image using the form on the homepage.
- View the uploaded image and its RGB arrays on the result page.

## License
MIT License
