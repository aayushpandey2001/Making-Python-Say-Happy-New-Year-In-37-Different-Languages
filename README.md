# Making-Python-Say-Happy-New-Year-In-37-Different-Languages
Making Python Say Happy New Year In 37 Different Languages


#-----------------------------------Project----------------------------------
from win32com.client import Dispatch

def speak(str):
    speak = Dispatch(("SAPI.SpVoice"))
    speak.Speak(str)

if __name__ == '__main__':
    with open("1.txt") as f:
        for item in f.readlines():
            speak(item)
        
