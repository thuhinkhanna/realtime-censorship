# Real-Time Censorship using Deep Learning

## Overview

The project is a browser extension to detect and redact NSFW content from web pages in real-time. Deep learning models for text and image classification are used to classify the content in the web pages after they are scraped. The text or image that is classified as not safe are blurred in the web page being displayed.

## Installation

1. Clone the repository. The repository should contain the files to setup the browser extension, text classification server and image classification server.
2. Setting up the text classification server.
   * The Express Server folder contains all the files for the text classification server.
   * Install the required packages for the Express app by running ```npm i```. This will install all the packages in the lockfile.
   * Once all the packages are installed run ```npm start``` to start the server.
3. Setting up the image classification server.
   * The Flask Server folder contains all the files and the saved model for the image classification server.
   * Create a python virtual environment by running the command ```virtualenv env```.
   * Activate the virtual environment by running ```source env/bin/activate```.
   * Install the required packages for the Flask app by running ```pip install -r requirements.txt```.
   * Once all the packages are installed run ```flask --app app.py --debug run``` to start the server.
4. Enable developer mode in your browser and install the extension from the Browser Extension folder using the Load unpacked feature.
5. Load into any page and run the browser extension on it.

## Demo Video

<iframe src="https://drive.google.com/file/d/1fJ_ETrYDe968CxkZ6eo-Q4IIlgwczwNv/preview" width="640" height="480"></iframe>

## Model Details
