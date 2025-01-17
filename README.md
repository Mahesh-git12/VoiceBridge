VoiceBridge: Voice-to-Text Translation Application
Description
VoiceBridge is a Python-based application designed to break language barriers. It captures voice input, converts it to text, identifies the language, translates the text into a user-specified language, and generates an audio output in the translated language.

Features
Captures voice input via microphone.
Recognizes spoken text using Google Speech Recognition.
Detects the language of the spoken text.
Translates text into a specified target language.
Converts translated text into an audio file using Google Text-to-Speech (gTTS).
Supported Languages
This application supports translation to:

Hindi (hi)
Telugu (te)
Kannada (kn)
Tamil (ta)
Malayalam (ml)
Bengali (bn)
Prerequisites
Before running the application, ensure the following are installed:

Python 3.7 or higher
Required Python Libraries
Install these dependencies using pip:

bash
Copy
Edit
pip install -r requirements.txt  
Contents of requirements.txt:

txt
Copy
Edit
speechrecognition  
googletrans==4.0.0-rc1  
gtts  
pyaudio  
Installation
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/voicebridge.git  
cd voicebridge  
Install the dependencies:

bash
Copy
Edit
pip install -r requirements.txt  
Ensure your microphone is connected and accessible.

Usage
Run the application:

bash
Copy
Edit
python app.py  
When prompted, enter the target language (e.g., Hindi, Telugu, Tamil).

Speak into the microphone when instructed.

The application will:

Recognize your speech.
Detect the language of your spoken text.
Translate it into the target language.
Save the translated audio file in the outputs directory.
The translated audio will automatically play if your system supports it.

File Structure
bash
Copy
Edit
voicebridge/  
│-- app.py                # Main application script  
│-- requirements.txt      # Required libraries  
│-- outputs/              # Folder for translated audio files  
Notes
Google Speech Recognition and GoogleTrans require an active internet connection.
The googletrans library may occasionally encounter issues. If translation fails, check your network connection or try again later.
Troubleshooting
PyAudio Not Found:
If you encounter a ModuleNotFoundError for PyAudio, install it as follows:

For Windows:
bash
Copy
Edit
pip install pipwin  
pipwin install pyaudio  
For macOS/Linux:
bash
Copy
Edit
brew install portaudio  
pip install pyaudio  
No Speech Recognized:

Ensure your microphone is working.
Speak clearly and avoid background noise.
Contributing
Feel free to fork this repository and contribute! Submit a pull request with any enhancements or bug fixes.

License
This project is licensed under the MIT License.

