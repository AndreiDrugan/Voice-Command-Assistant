# Voice Command Assistant

A local voice assistant built in Python that combines **OpenAI Whisper** for speech-to-text transcription with TF-IDF vectorization and cosine similarity to map transcribed phrases to system commands.

## Prerequisites

* Python 3.10 or a newer version
* FFmpeg (mandatory for audio and video file decoding)

## Installation

   Install FFmpeg on Windows via terminal:
   ```bash
   winget install Gyan.FFmpeg
   ```
   Install the required Python dependencies:
   ```bash
   pip install openai-whisper scikit-learn pandas numpy
   ```
## Project Structure
main.ipynb - The primary Jupyter Notebook containing the end-to-end pipeline: transcription, TF-IDF vectorization, cosine similarity calculation, and command routing.

comenzi.csv - The local dataset linking reference sentences to specific command identifiers.

## Usage
Place your target audio or video file (such as db.mp4) directly inside the project directory.

Open the Jupyter Notebook and execute the cells sequentially to load the Whisper model, process the input text, determine the best intent match, and trigger the corresponding action through subprocess or webbrowser.
