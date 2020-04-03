# Finding-EMO
An app which identifies the human emotion using acoustic features in real time.

Five classes of emotion is identified : Happy, sad, angry, neutral and fear.


Android has a built-in microphone through which  can capture audio and store it , or play it on the phone. Audio is recorded in PCM format (raw file). It is then converted from PCM to Wav by adding proper header.
 
Audio signal is then preprocessed and 12 MFCC coeficients are extracted using python script and CNN model is trained.


Model is deployed and bundled with apk with the help of chaquopy.


Using the trained model , recorded audio files should be  processed, inference on input data should be  performed and recognised emotion will be displayed through the app.


App screenshots are available in images folder.


PS: Couldn't upload entire apk source files as python library files are too large.
