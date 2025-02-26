# AI-DUBBING
AI powered multilingual audio and video dubbing

### Tools, Models, and Libraries Used

| Category                          | Tool/Model/Library                          | Purpose in Project |
|-----------------------------------|--------------------------------------------|--------------------|
| **File Upload & Handling**        | ipywidgets                                 | Allows users to **upload** audio or video files easily. |
| **Media Processing**              | ffmpeg-python                             | 1. **Extracts audio** from video. 2. **Merges dubbed audio** back into video. |
| **Speech-to-Text (ASR)**          | Whisper (openai/whisper-large-v3)         | Converts **spoken words into text** with high accuracy. |
| **Text Translation**              | NLLB-200 (facebook/nllb-200-distilled-600M) | Translates transcribed text into a **user-selected language** (supports 200+ languages). |
| **Text-to-Speech (TTS) - Voice Generation** | gTTS (Google Text-to-Speech) | Converts **translated text into speech** in the target language. |
| **Audio Processing**              | pydub                                     | Processes and **converts audio formats**, adjusts volume, and trims audio. |
| **Merging Dubbed Audio with Video** | ffmpeg-python                             | Ensures **synchronized replacement** of original audio with dubbed audio. |
| **Downloading Output**            | ipywidgets                                | Provides a **download option** for the final dubbed audio/video. |
| **Model Hosting & Access**        | Hugging Face Hub                          | Stores and accesses **pre-trained models** (Whisper, NLLB-200). |
| **User Interface**                | Gradio                                   | Creates a **user-friendly web interface** to upload files, select languages, and get results. |


Project WorkFlow:
1.	Upload video or Audio file(via Gradio interface)
2.	Extract Audio from video using FFmpeg
3.	Transcribe Sppech to Text using Whisper
4.	Translate Text into Target Language using NLLB-200
5.	Convert Translated Text to Speech using gTTS.
6.	Synchronize Dubbed Audio with Video using FFmpeg.
7.	Generate the final Dubbed Video/Audio for download.

Type 	Supported Extensions
Video	.mp4, .avi, .mkv, .mov, .webm, .flv
Audio	.mp3, .wav, .ogg, .flac, .aac, .m4a

