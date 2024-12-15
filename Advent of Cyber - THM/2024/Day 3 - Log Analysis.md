# Task 9 - Log analysis Day 3: Even if I wanted to go, their vulnerabilities wouldn't allow it.

## Learning Objectives
- Learn about Log analysis and tools like ELK.
- Learn about KQL and how it can be used to investigate logs using ELK.
- Learn about RCE (Remote Code Execution), and how this can be done via insecure file upload.

http://10.10.45.227:5601/app/home#/
```bash
echo "10.10.104.113 frostypines.thm" >> /etc/hosts
```

<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-1.png" alt="day3-1"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-2.png" alt="day3-2"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-3.png" alt="day3-3"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-4.png" alt="day3-4"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-5.png" alt="day3-5"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-6.png" alt="day3-6"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-7.png" alt="day3-7"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-8.png" alt="day3-8"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-9.png" alt="day3-9"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-10.png" alt="day3-10"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-11.png" alt="day3-11"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-12.png" alt="day3-12"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-13.png" alt="day3-13"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-14.png" alt="day3-14"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-15.png" alt="day3-15"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-16.png" alt="day3-16"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-17.png" alt="day3-17"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-18.png" alt="day3-18"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-19.png" alt="day3-19"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day3-20.png" alt="day3-20"><br>

