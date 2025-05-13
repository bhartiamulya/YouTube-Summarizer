# YouTube Lecture Summarizer Backend

This backend enables summarization of any YouTube video, even those without transcripts, by downloading audio, transcribing with Whisper, and summarizing with a Hugging Face model.

## Features
- Accepts YouTube URLs via REST API
- Downloads audio using yt-dlp
- Transcribes audio to text using Whisper
- Summarizes transcript using BART/T5
- (Optional) Translates summary using LibreTranslate

## Setup
1. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
2. Run the server:
   ```
   uvicorn main:app --reload
   ```

## API Usage
- `POST /summarize` with JSON: `{ "youtube_url": "...", "target_lang": "en" }`
- Returns: `{ "summary": "...", "translated_summary": "..." }`

## Notes
- First run may be slow (model downloads)
- Whisper requires ffmpeg installed on your system
- For best results, use on videos with clear audio
