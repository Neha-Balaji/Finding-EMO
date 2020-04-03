# Finding-EMO
An app which identifies the human emotion using acoustic features in real time.



Input: Recorder audio
Output: Recognized emotion
Steps: 
    Android app development 
    Deployment of Trained model
    Recording audio
    Conversion from PCM to WAV
    Preprocessing and feature extraction
    Emotion recognition

Recording audio
Frontend : Android app recording audio
Input : Audio file in raw PCM format
Android has a built-in microphone through which  can capture audio and store it , or play it on the phone. Audio is recorded in PCM format (raw file). 

Conversion from PCM to Wav
Input : Realtime audio recorded in pcm format.
Output : .wav audio file (WAV = Metadata  - RIFF file, fmt data + PCM raw byte) 
Steps :
    Opens up the given file, writes the header, and keeps filling it with raw PCM bytes from AudioRecord until it reaches a certain size  or is stopped by the user. 
    Then updates the WAV header to include the proper final chunk sizes.
    Writes the proper 44-byte RIFF/WAVE header to/for the given stream
    Updates the given wav file's header to include the final chunk sizes

Preprocessing and feature extraction is done using python code. 12 MFCC coeficients are extracted and model is trained.

Deployment of trained model
Input: Trained model
Output: Model bundled with app using python script
Steps:
    Add chaquopy to android studio (To create python instance to be called from java)
    Install required packages
    Pick a pre-trained keras model
    Bundle it with python script
    Create python instance and invoke python script


Emotion Recognition
Using the trained model , recorded audio files should be  processed, inference on input data should be  performed and recognised emotion will be displayed through the app.



Training Model summary

