# YouTube Lecture Summarizer Chrome Extension

This Chrome extension extracts transcripts from YouTube videos, creates summaries, and allows translation to different languages.

## Features
- Extracts transcripts from YouTube videos with captions
- Summarizes lecture content using frequency-based extraction
- Translates summaries to multiple languages
- Downloads summaries as text files
- Persistent side panel with draggable interface
- Close and minimize buttons for better user experience

## Setup
1. Clone this repository
2. Install backend requirements:
   ```
   cd youtube-lecture-backend
   pip install -r requirements.txt
   python main.py
   ```
3. Load the extension in Chrome:
   - Go to `chrome://extensions/`
   - Enable Developer Mode
   - Click "Load unpacked" and select the `youtube-lecture-summarizer` folder

## How to Use
1. Navigate to a YouTube video with captions
2. Click the extension icon to open the side panel
3. Click "Summarize" to generate a summary
4. Select a language and click "Translate" to translate the summary
5. Use "Copy" to copy the text or "Save as Text" to download it
6. Drag the panel header to reposition it on screen
7. Use the X button to close the panel when not needed

## Requirements
- Python 3.6+
- NLTK
- youtube-transcript-api
- FastAPI
- Chrome browser
