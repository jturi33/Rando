# Rando
//SslReverseLib is a copy of Jamie Bowman's reverse shell implementation (Ref #1).
The only change I made was wrapping it inside of Microsoft's official SSLSTREAM class (Ref #2).
Programmer needs only to provide a base64 encoded PEM certificate to get it working
1. https://www.mrjamiebowman.com/hacking/c-sharp-reverse-shell/
2. https://docs.microsoft.com/en-us/dotnet/api/system.net.security.sslstream

//HexecutableInvoker executes any hexecutable program provided. 
It was inspired by a SANS article on malicious JavaScript (Ref #1) as well Reversing Hub's exquisite class on hexecutable malware. Reccomend highly!!! (Ref #2).
The programmer needs only to replace the namespace & class with that of their implemented program & then provide the necessary arguments. Convert your program to .hex format using the instructions provided in ReversingHub's Udemy course linked below.
1. https://isc.sans.edu/forums/diary/Malicious+Script+With+Multiple+Payloads/25090/
2. https://www.udemy.com/course/reverse-engineering-deep-dive/

//Powershell Dropper
JavaScript file take a URL leading a .txt file. This file should contain PowerShell commands seperated by semicolon and will be ran by PowerShell upon execution of
the script.

//VBA Macro Hacker
Originally derived from the below StackOverflow page (Ref #1) this .csv contains a function to unlock any VBA macro past password protection.
Open the MacroHacker.csv along side your favorite password protected macro & then execute the unlock funtion.
This should make the previously locked macro viewable in Excel's VBA editor.
1. https://stackoverflow.com/questions/1026483/is-there-a-way-to-crack-the-password-on-an-excel-vba-project
