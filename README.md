# YouTube Lecture Summarizer

A tool to automatically summarize YouTube lecture videos, making it easier for students and learners to review and understand educational content.

## Overview

The YouTube Lecture Summarizer is a two-part application:

1. **Backend API** - A Python-based service that processes YouTube videos and generates summaries
2. **Frontend Extension** - A browser extension that integrates with YouTube to provide summaries directly on the video page

## Features

- Extract and summarize content from YouTube lecture videos
- Generate concise text summaries of lengthy educational content
- Browser extension for seamless integration with YouTube
- Support for various lecture formats and topics

## Tech Stack

### Backend
- Python
- FastAPI
- YouTube transcript API
- Natural Language Processing libraries

### Frontend
- JavaScript
- HTML/CSS
- Chrome Extension API

## Installation

### Backend Setup

1. Navigate to the backend directory:
   ```
   cd youtube-lecture-backend
   ```

2. Create a virtual environment:
   ```
   python -m venv venv
   ```

3. Activate the virtual environment:
   - Windows: `venv\Scripts\activate`
   - Mac/Linux: `source venv/bin/activate`

4. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

5. Run the server:
   ```
   python main.py
   ```

### Frontend Setup

1. Navigate to the frontend directory:
   ```
   cd youtube-lecture-summarizer
   ```

2. Load the extension in Chrome:
   - Open Chrome and go to `chrome://extensions/`
   - Enable "Developer mode"
   - Click "Load unpacked" and select the extension directory

## Usage

1. Navigate to a YouTube lecture video
2. Click on the extension icon in your browser
3. The extension will process the video and display a summary

## Project Structure

```
youtube-summarizer/
├── youtube-lecture-backend/    # Backend API service
│   ├── main.py                 # Main application entry point
│   ├── summarizer.py           # Core summarization logic
│   └── requirements.txt        # Python dependencies
│
└── youtube-lecture-summarizer/ # Frontend browser extension
    ├── manifest.json           # Extension configuration
    ├── popup.html              # Extension popup interface
    ├── popup.js                # Extension logic
    ├── content.js              # Content script for YouTube integration
    └── background.js           # Background script for extension
```

## Future Improvements

- Add support for multiple languages
- Implement more advanced summarization algorithms
- Add user customization options for summary length and style
- Support for additional video platforms beyond YouTube

## Contact

Amulya Bharti J - bhartiamulya0902@gmail.com

