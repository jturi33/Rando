# Rando
//SslReverseLib
SslReverseLib is a copy of some security researches reverse shell implementation (please comment if you can find the link I seem to have lost it).
The only change I made was wrapping it inside of Microsoft's official SSLSTREAM class.
The hacker need only provide a base64 encoded PEM certificate to get it working.

//HexecutableInvoker
The Hexecutable invoker executes any hexecutable program provided. 
It was inspired by a SANS article on malicious JavaScript as well Reversing Hub's exquisite class on hexecutable malware. Reccomend highly!!!
The hacker needs only to replace the namespace & class with that of their implemented program & then provide the necessary arguments convert their program to .hex format (See ReversingHub's course linked below) &
then replace arg1 & arg2 with the necessery argument's to execute the specified function (assuming they aren't 'args 1 & 2').

//Powershell Dropper
JavaScript file take a URL leading a .txt file. This file should contain PowerShell commands seperated by semicolon and will be ran by PowerShell upon execution of
the script.

//VBA Macro Hacker
Originally derived from the below StackOverflow article this .csv contains a function to unlock any VBA macro past password protection.
Open the MacroHacker.csv along side your favorite password protected macro & then execute the unlock funtion.
This should make the previously locked macro viewable in Excel's VBA editor.

References:

