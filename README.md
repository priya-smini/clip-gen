# clip-gen

A smart assistant for video creators to turn long content into short clips — and auto-schedule them to Shorts/YouTube/Instagram.

## Business Logic
Input: YouTube video link
Step 1: Download the video
Step 2: Transcribe using OpenAI Whisper
Step 3: Extract 1–2 highlight clips (based on timestamps, e.g. every 30–60 seconds)
Step 4: Export clips as MP4 files

## Tech Stack
Python
pytube – Download YouTube videos
whisper – Transcribe speech to text
moviepy – Video editing (clip cutter)

### Setup
brew install ffmpeg
python3 -m venv venv
source venv/bin/activate

pip install pytube moviepy openai-whisper 
pip install torch (required for whisper)

pip install jupyter
jupyter notebook
