<h1>Setting Up Whisper AI: Installation & Tools</h1>
To get started with Whisper AI, I followed these simple steps in my Google Collab Notebook and changed the runtime type to T4 GPU:

<h2>1. Installing Whisper AI</h2>
Whisper isn’t available via pip install whisper, so you need to install it directly from GitHub:
pip install git+https://github.com/openai/whisper.git

<h2>2. Installing FFmpeg</h2>
Since Whisper processes audio, it requires FFmpeg, which can be installed using:
!sudo apt update && sudo apt install ffmpeg

<h2>3. Running Whisper AI on a Video File</h2>
Once the setup was complete, I ran Whisper on a sample video file to generate captions:
!whisper “file_name.mp4” — model medium
This command automatically transcribed the audio from the video and generated subtitles!
The captions are stored in filename.txt and filename.srt files.

<h2>4. Running Whisper AI on a Audio File</h2>
Then I also ran whisper AI on an audio which contains poetry from Hindi/Urdu language and I asked for the english translation. And I got it.
The following command generated the captions in English
!whisper “audio_file.mp3” — model medium — language English
