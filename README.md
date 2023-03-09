# Text-to-speech
#text to speech convert by using python (text reader)


#What is text-to-speech ? 

#Text-to-speech (TTS) refers to the ability of computers to read text aloud. A TTS engine converts written text to a phonemic representation, then converts the #phonemic representation to waveforms that can be output as sound.







                            # we have imported this module is help to text to speech conversion
                            from gtts import gTTS
                            import os

                            abc = open("sample.txt")

                            # text that you want to convert
                            text = abc.read()

                            # en is stand for english language
                            language ="en"


                            # we have used slow  = False because our converted video will have a high speed
                            obj =gTTS(text=text , lang=language , slow=False)

                            obj.save("sample.mp3")


                            # to open the video file automatically we import os module
                            os.system("sample.mp3")



