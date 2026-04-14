# Voice_Authentication_System

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

Languages & Tools
-
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) 
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![Librosa](https://img.shields.io/badge/Librosa-blue?style=for-the-badge&logo=python&logoColor=white)
![OpenAI Whisper](https://img.shields.io/badge/OpenAI%20Whisper-412991?style=for-the-badge&logo=openai&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)

Project Structure
-
```text
Project Voice_Authentication/
├── Project_VA/
│   ├── recordings/ 
│   │   └── Instructions.md
│   ├── Static
│   │   ├── CSS_Styling.css
│   │   └── Unified_Html.html
│   ├── app/
│   │   ├── audio_utils.py
│   │   ├── database.py
│   │   ├── main.py
│   │   └── voice_matcher.py
│   ├── add_student.py
│   ├── requirements.txt
│   └── README.md
```

Setup Instructions
-
[![Clone this repo](https://img.shields.io/badge/Clone-This_Repo-blue?style=for-the-badge&logo=github)](https://github.com/Amazingly12/Voice_Authentication_System/archive/refs/heads/main.zip)

1. Clone the Repository.
   ```Text
    git clone [https://github.com/Amazingly12/Voice_Authentication_System.git](https://github.com/Amazingly12/Voice_Authentication_System.git)
    ```

2. Go into Project Directory, Create and activate a virtual environment.
   ```Text
   cd Project_VA
   python -m venv .venv
   .\.venv\Scripts\activate   
   ```

3. Install requirements and Dependencies.
   ```Text
   pip install -r requirements.txt
   ```

Database Setup
-
This Project uses MongoDB Compass as primary data store.
1. Install MongoDB Compass: [Download here](https://www.mongodb.com/try/download/shell).
2. Connection: Open MongoDB Compass.
   - Click "New Connection".
   - Paste the following link:
     ```Text
     mongodb://localhost:27017
     ```
   - Click Connect.
3. The Database will automatically create a database (it should be named as VoiceAuthDB).

Run the Application
-
After Installing Requirements, Creating your own local Database on MongoDB, you can run the application
```Text
#Ensure you are in the correct Directory (Project_VA) and have the .venv activated.
uvicorn app.main:app --reload
```

Screenshots
-
