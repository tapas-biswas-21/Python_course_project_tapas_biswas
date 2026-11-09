# Python_course_project_tapas_biswas

An AI-based web application built with Python, Flask, and embeddable Watson NLP libraries to perform fine-grained emotion analytics on customer feedback text. This project extracts specific emotional states (anger, disgust, fear, joy, sadness) and determines the dominant emotion.

## Project Structure
* `server.py` - Core Flask application web deployment controller.
* `EmotionDetection/` - Python package containing modules for connecting to the Watson NLP API.
  * `__init__.py` - Package initialization file.
  * `emotion_detection.py` - Core logic for making API calls and formatting the text analysis output.
* `test_emotion_detection.py` - Automated unit testing suite.
* `templates/index.html` - Client-side user interface web interface layout.

## Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd Python_course_project_tapas_biswas
   ```

2. **Install required dependencies:**
   ```bash
   pip install requests flask pylint
   ```

3. **Run Unit Tests:**
   ```bash
   python3 test_emotion_detection.py
   ```

4. **Launch the Flask Application Server:**
   ```bash
   python3 server.py
   ```
   Access the local web interface on `http://localhost:5000` via your web browser.

## API Documentation
The application exposes a RESTful web application endpoint at `/emotionDetector` which takes a `textToAnalyze` query argument string and returns a structured breakdown of raw scores alongside the dominant emotional trait.
