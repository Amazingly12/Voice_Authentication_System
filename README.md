# Voice_Authentication_System

Overview
-
A secure voice authentication system built with FastAPI that uses voice biometrics and challenge-response verification to authenticate users. Users are enrolled by uploading voice samples, and verified by speaking randomly generated phrases checked for both speaker identity and phrase accuracy.

Security Measures
-
Challenges restricts pre-recorded playback. System verifies and nullifies AI voice assistants. Whisper adds robustness to transcription across accents and noise.

Features
-
- Voice-based user authentication
- Live microphone recording via browser
- Challenge phrase validation
- Speech-to-text transcription using OpenAI Whisper
- MongoDB database for storing user voiceprints
- Clean HTML UI with a minimal dark theme
- FastAPI (Python)
