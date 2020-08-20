# SimplePyTask1
## Made a Simple cmd application which will launch application allowing users to type what they want to open 
### Giving speaking assistance as well!
## Here I used library pyttsx3 for voiceover kind of for whatever commands given.
The code looks like this :
import os
import pyttsx3 as spkk



print(" CAN  I HELP YOU?")


def jvs(a):
	spkk.speak("gottcha....."+a+"..launching for you!")
	spkk.speak("If Anything else..I am still here to help you")

spkk.speak("Ooh,... Great to see you again! Can I help you.. with anything?..Just Type here")

while True:
	x = input(" Just type : ")
	if ("notepad" in x):
		y = "notepad"
		jvs("notepad")
		os.system(y)
		print(y+ "..LAUNCHED..")
	elif ("calculator" in x):
		y = "calc"
		jvs("calculator")
		os.system(y)
		print(y+ "..LAUNCHED..")
	elif ("paint" in x):
		y = "mspaint"
		jvs("Paint")
		os.system(y)
		print(y+"..LAUNCHED..")

	elif ("media player" in x):
		y = "wmplayer"
		jvs("Media player")
		os.system(y)
		print(y + "..LAUNCHED..")
	elif ("taskmanager" in x):
		y = "taskmgr"
		jvs("Task manager")
		os.system(y)
		print(y + "..LAUNCHED..")
	elif ("exit" in x):
		y = "exit"
		spkk.speak("Exitting....Come...again..")
		print("Exitted Come Again")
		break
	else:
		spkk.speak("Something is wrong! Try again")
		print("Something is wrong! Try again")




