# Menu-driven-system-apps
import os
import pyttsx3


while True:
    y=['Paint','Word','Notepad++','Notepad','vlc','Google','Calculator','Windows Media Player','Edit image','Clock','Calendar','Excel','PPT','Atom']

    print("\nI can help you with running the programs listed\n",*y, sep='\n  ')
    pyttsx3.speak('I can help you with running the programs listed')
    print('\nHow can I help U:\n')
    pyttsx3.speak('How can i help you')

    x=input()
    print('Thankyou :)')
    if (("run" in x) or ("execute"in x) or ("open"in x)) and (("google"in x)or("chrome" in x)):
        if 'Google' in y or 'chrome' in y:
            s=input("Website:")
            os.system('chrome '+s)
            pyttsx3.speak("chrome is opened for u")
        else:
            pyttsx3.speak("sorry desired application is not available")
    elif ((("run" in x) or ("execute"in x) or ("open"in x) or ("play"in x)) and (("video player"in x)or("vlc player" in x)or("videos"in x))):
        if 'vlc' in y:
            os.system('vlc')
            pyttsx3.speak("vlc player is opened for u")
        else:
            pyttsx3.speak("sorry desired application is not available")
    elif ((("run"in x) or ("execute"in x) or ("open"in x)or("play"in x)) and (("player"in x)or("media player" in x)or("wmplayer"in x)or("media"in x))):
        if 'Windows Media Player' in y:

            os.system('wmplayer')
            pyttsx3.speak("Windows media is opened for u")
        else:
            pyttsx3.speak("sorry desired application is not available")
    elif ((("run"in x) or ("execute"in x) or ("open"in x)) and (("msword"in x)or("word" in x)or("document"in x))):
        if 'Word' in y:
            os.system("winword")
            pyttsx3.speak("word is opened for u")
        else:
            pyttsx3.speak("sorry desired application is not available")
    elif ((("run"in x) or ("execute"in x) or ("open"in x)) and (("notepad++"in x)or("code editor" in x)or("code"in x))):
        if 'Notepad++'in y:
            os.system("notepad++")
            pyttsx3.speak("notepad++ is opened for u")
        else:
            pyttsx3.speak("sorry desired application is not available")
    elif ((("notepad" in x) or ("text editor" in x)or ("notes"in x))and (("open"in x) or ("run"in x))) :
        if 'Notepad'in y:
            pyttsx3.speak("notepad is opened for u")
            os.system("notepad")
        else:
            pyttsx3.speak("sorry desired application is not available")
    elif ((("paint"in x)or("draw"in x)or("mspaint"in x))and(("open"in x)or("show"in x)or("run"in x))):
        if 'Paint' in y:
            pyttsx3.speak("paint is opened for u")
            os.system("mspaint")
        else:
            pyttsx3.speak("sorry desired application is not available")
    elif (("edit"in x or "crop"in x or 'view'in x)and("image"in x or "images"in x or "pictures"in x or "picture" in x or "imgs"in x or "img"in x or "pic"in x or "pics"in x)or("open"in x or "show"in x or "run"in x)):
        if 'Edit image' in y:
            pyttsx3.speak("Image editor is opened for u")
            os.system("start ois")
        else:
            pyttsx3.speak("sorry desired application is not available")
    elif ((("run" in x) or ("execute"in x) or ("open"in x) or ("show"in x)) and (("calendar "in x)or("date" in x)or("month"in x))):
        if 'Calendar' in y:
            os.system('start outlookcal:')
            pyttsx3.speak("calendar is opened for u")
        else:
            pyttsx3.speak("sorry desired application is not available")
    elif ((("run" in x) or ("display"in x)or ("set"in x) or ("open"in x) or ("show"in x)) and (("alarm"in x)or("time" in x)or("stopwatch"in x)or("timer"in x)or("clock"in x))):
        if 'Clock' in y:
            os.system('start ms-clock:')
            pyttsx3.speak("Clock and Alarm is opened for u")
        else:
            pyttsx3.speak("sorry desired application is not available")
    elif ((("run" in x) or ("display"in x)or ("execute"in x) or ("open"in x) or ("show"in x)) and (("calculator"in x)or("calculations" in x)or("calculation"in x))):
        if 'Calculator' in y:
            os.system('start calculator:')
            pyttsx3.speak("Calculator is opened for u")
        else:
            pyttsx3.speak("sorry desired application is not available")
    elif ((("run" in x) or ("display"in x)or ("open"in x) or ("show"in x)) and (("code"in x)or("atom" in x)or("editor"in x))):
        if 'Atom' in y:
            os.system('start atom')
            pyttsx3.speak("Atom is opened for u")
        else:
            pyttsx3.speak("sorry desired application is not available")
    elif ((("run"in x) or ("execute"in x) or ("open"in x)) and (("msexcel"in x)or("sheets" in x)or("excel"in x))):
        if 'Excel' in y:
            os.system("start excel")
            pyttsx3.speak("MS Excel is opened for u")
        else:
            pyttsx3.speak("Sorry desired application is not available")
    elif ((("run"in x) or ("execute"in x) or ("open"in x)) and (("ms power point"in x)or("slides" in x)or("power point"in x)or("slides"))):
        if 'PPT' in y:
            os.system("start powerpnt")
            pyttsx3.speak("Powerpoint is opened for u")
        else:
            pyttsx3.speak("Sorry desired application is not available")

    elif 'exit' in x:
        break
    else:
        pyttsx3.speak("Sorry, desired application is not available. Thank you for your approach")
        break
