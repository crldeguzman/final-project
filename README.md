# Emotion Detector

Emotion Detector is a Flask web application that sends English text to the IBM
Skills Network Watson emotion service and displays the detected emotions. It
reports scores for **anger**, **disgust**, **fear**, **joy**, and **sadness**,
then identifies the emotion with the highest score as the dominant emotion.

## Technologies

- Python 3
- Flask
- Requests
- IBM Skills Network Watson emotion endpoint
- HTML, JavaScript, and Bootstrap

## Installation

From the repository root, create and activate a virtual environment if desired,
then install the required packages:

```powershell
python -m pip install Flask requests pylint
```

## Run the application

```powershell
python server.py
```

Open `http://127.0.0.1:5000/` in a browser.

## Run unit tests

The tests call the course-required IBM Skills Network endpoint, so an internet
connection is required.

```powershell
python -m unittest test_emotion_detection.py -v
```

## Run Pylint

```powershell
python -m pylint server.py
python -m pylint EmotionDetection/emotion_detection.py
```
