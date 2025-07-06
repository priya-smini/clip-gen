# 🎬 clip-gen

A smart assistant for video creators to turn long-form videos into short, viral-ready clips — and auto-schedule them to YouTube Shorts, Instagram Reels, or other platforms.

---

## 🧠 Business Logic

🔗 **Input**: YouTube video link  
🔽 **Step 1**: Download the video  
🗣️ **Step 2**: Transcribe using OpenAI Whisper  
✂️ **Step 3**: Extract 1–2 highlight clips (based on timestamps, e.g., every 30–60 seconds)  
📤 **Step 4**: Export clips as `.mp4` files  

---

## 🧰 Tech Stack

- 🐍 **Python**
- 📥 [`pytube`](https://pytube.io/) – Download YouTube videos
- 🧠 [`whisper`](https://github.com/openai/whisper) – Transcribe speech to text
- 🎞️ [`moviepy`](https://zulko.github.io/moviepy/) – Video editing (clip cutter)
- 🔧 `ffmpeg` – Backend video processing tool

---

## ⚙️ Setup Instructions (MacOS)

## ⚙️ Setup Instructions (MacOS)

```bash
brew install ffmpeg

python3 -m venv venv
source venv/bin/activate

pip install pytube moviepy openai-whisper
pip install torch  # required for whisper
pip install jupyter

jupyter notebook

