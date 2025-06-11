# Multilingual audio visual system with lip synchronization using GAN
 # Multilingual-to-English Lip-Synced Video Translation using Wav2Lip

🎥🗣️ This project takes a **video in any language** and generates a new **English-speaking video** where the subject’s lip movements are **perfectly synchronized** with translated English audio. By combining **ASR (Automatic Speech Recognition)**, **Translation**, **Text-to-Speech (TTS)**, and the **Wav2Lip** model, it offers a powerful tool for multilingual video dubbing, accessibility, and global content delivery.

---

## 🎯 Features

- 🌐 **Multilingual Input Video**: Accepts videos with speech in languages like Hindi, Malayalam, Spanish, etc.
- 🔁 **Automatic Speech Translation**: Converts the original speech to English using ASR + Translation.
- 🔊 **English Audio Generation**: Uses TTS to produce natural English speech from translated text.
- 👄 **Lip-Sync with Wav2Lip**: Ensures the face in the original video speaks English with accurate, expressive lip movements.
- 📦 **Video-to-Video Pipeline**: Input video → Output video (same speaker, new audio & synced lips).

---

## 🏗️ System Architecture

1. 🎬 **Input Video** (any language)
2. 🔊 **Audio Extraction**
3. 🧠 **Speech-to-Text (ASR)**: Transcribe spoken content using models like `Whisper`.
4. 🌍 **Translation**: Translate transcribed text to English using Google Translate or MarianMT.
5. 🔈 **Text-to-Speech**: Generate English audio from translated text (e.g., with `gTTS`).
6. 👄 **Lip Sync (Wav2Lip)**: Use English audio + original video to synthesize synced mouth movements.
7. 🎞️ **Video Generation**: Combine output frames into a new video with English speech and lip sync.

---

## 🧪 Requirements

- Python 3.8+
- PyTorch
- OpenCV
- NumPy
- librosa
- moviepy
- ffmpeg
- tqdm
- [Wav2Lip](https://github.com/Rudrabha/Wav2Lip)
- whisper / other ASR tools
- gTTS or pyttsx3 for TTS
- Google Translate API or MarianMT for translation

### 📦 Install all dependencies:

```bash
pip install -r requirements.txt
