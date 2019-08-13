# Voice Recognition

## Introduction to Mozilla Deep Speech

Mozilla Deep Speech is Mozilla’s implementation of Baidu’s Deep Speech [1] Neural Network Architecture. It is designed for various reasons:

- open state-of-the-art alternative to proprietary solutions such as Amazon Alex, Google Assistant or Baidu …
- offline support
- privacy
- low latency
- works in “disconnected” settings, e.g. industrial control systems that are detached for good reasons or mobile devices experiencing insufficient network coverage
    scaleable

## How to use  Mozilla Deep Speech

Open notebook after login to  https://nbai.io

Open a terminal and type

`
git clone https://github.com/nebulaai/voice-recognition.git
`

You can use  Speech_To_Text.ipynb for converting a speech to text, you need to replace _downloads/speech.mp3_ with the file name you used in the following commind in the cell

`
!ffmpeg -i downloads/speech.mp3 -vn -acodec pcm_s16le -ac 1 -ar 16000 -f wav downloads/speech.wav
`

## References

[1] Hannun et al. (2014): Deep Speech: Scaling up end-to-end speech recognition. arXiv: 1412.5567
