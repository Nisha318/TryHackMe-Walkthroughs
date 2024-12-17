# Sandboxes Day 6: If I can't find a nice malware to use, I'm not going.

## Learning Objectives
- Analyze malware behaviour using sandbox tools.
- Explore how to use YARA rules to detect malicious patterns.
- Learn about various malware evasion techniques.
- Implement an evasion technique to bypass YARA rule detection.


<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-1.png" alt="day6-1"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-2.png" alt="day6-2"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-3.png" alt="day6-3"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-4.png" alt="day6-4"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-5.png" alt="day6-5"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-6.png" alt="day6-6"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-7.png" alt="day6-7"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-8.png" alt="day6-8"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-9.png" alt="day6-9"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-10.png" alt="day6-10"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-11.png" alt="day6-11"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-12.png" alt="day6-12"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-13.png" alt="day6-13"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-14.png" alt="day6-14"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-15.png" alt="day6-15"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-16.png" alt="day6-16"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-17.png" alt="day6-17"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-18.png" alt="day6-18"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-19.png" alt="day6-19"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-20.png" alt="day6-20"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-21.png" alt="day6-21"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-22.png" alt="day6-22"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-23.png" alt="day6-23"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-24.png" alt="day6-24"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-25.png" alt="day6-25"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-26.png" alt="day6-26"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-27.png" alt="day6-27"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day6-28.png" alt="day6-28"><br>



What is the flag displayed in the popup window after the EDR detects the malware?

- THM{GlitchWasHere}
 
What is the flag found in the malstrings.txt document after running floss.exe, and opening the file in a text editor?

- THM{HiddenClue}
 




