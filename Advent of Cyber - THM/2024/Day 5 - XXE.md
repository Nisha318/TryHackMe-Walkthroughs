# Task 11 - XXE Day 5: SOC-mas XX-what-ee?

## Learning Objectives
- Understand the basic concepts related to XML handling data like a file drawer.
- Explore XML External Entity (XXE) and its components
- Learn how to exploit the vulnerability
- Understand remediation measures

<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-1.png" alt="day5-1"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-2.png" alt="day5-2"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-3.png" alt="day5-3"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-4.png" alt="day5-4"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-5.png" alt="day5-5"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-6.png" alt="day5-6"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-7.png" alt="day5-7"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-8.png" alt="day5-8"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-9.png" alt="day5-9"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-10.png" alt="day5-10"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-11.png" alt="day5-11"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-12.png" alt="day5-12"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-13.png" alt="day5-13"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-14.png" alt="day5-14"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-15.png" alt="day5-15"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-16.png" alt="day5-16"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-17.png" alt="day5-17"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-18.png" alt="day5-18"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-19.png" alt="day5-19"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-20.png" alt="day5-20"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-21.png" alt="day5-21"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-22.png" alt="day5-22"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-23.png" alt="day5-23"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-24.png" alt="day5-24"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day5-25.png" alt="day5-25"><br>


What is the flag discovered after navigating through the wishes?
- THM{Brut3f0rc1n6_mY_w4y}
What is the flag seen on the possible proof of sabotage?
- THM{m4y0r_m4lw4r3_b4ckd00rs}
If you want to learn more about the XXE injection attack, check out the XXE room! 
- No answer needed <br>
Following McSkidy's advice, Software recently hardened the server. It used to have many unneeded open ports, but not anymore. Not that this matters in any way.
- No answer needed
