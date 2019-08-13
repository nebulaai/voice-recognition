# voice-recognition
voice recognition research using NBAI Cloud Notebook

Using Speech_To_Text.ipynb for training a speech to text, you need to change the following command if you use a different video file name

`
!ffmpeg -i downloads/speech.mp3 -vn -acodec pcm_s16le -ac 1 -ar 16000 -f wav downloads/speech.wav
`
