# Task 10 Atomic Red Team Day 4: I’m all atomic inside!

## Learning Objectives
- Learn how to identify malicious techniques using the MITRE ATT&CK framework.
- Learn about how to use Atomic Red Team tests to conduct attack simulations.
- Understand how to create alerting and detection rules from the attack tests.

<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-1.png" alt="day4-1"><br>

```bash
Get-Help Invoke-AtomicTest
```

<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-2.png" alt="day4-2"><br>

```bash
Invoke-AtomicTest T1566.001 -TestNumbers 2 -CheckPrereq
```
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-3.png" alt="day4-3"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-4.png" alt="day4-4"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-5.png" alt="day4-5"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-6.png" alt="day4-6"><br>

```bash
Invoke-AtomicTest T1566.001 -TestNumbers 1 -CheckPrereq
```

<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-7.png" alt="day4-7"><br>

```bash
Invoke-AtomicTest T1566.001 -TestNumbers 2 -CheckPrereq
```
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-8.png" alt="day4-8"><br>


<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-9.png" alt="day4-9"><br>

## Detecting the Atomic

```bash
Invoke-AtomicTest T1566.001 -TestNumbers 1 -cleanup
```

<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-10.png" alt="day4-10"><br>

Right-click Start > Event Viewer > Applications and Services Logs > Microsoft > Windows > Sysmon > Operational

<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-11.png" alt="day4-11"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-12.png" alt="day4-12"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-13.png" alt="day4-13"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-14.png" alt="day4-14"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-15.png" alt="day4-15"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-16.png" alt="day4-16"><br>

## Alerting on the Atomic
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-17.png" alt="day4-17"><br>


https://attack.mitre.org/techniques/T1059/
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-18.png" alt="day4-18"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-19.png" alt="day4-19"><br>
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-20.png" alt="day4-20"><br>

<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-20.png" alt="day4-21"><br>

```bash
 Invoke-AtomicTest T1059.003 -TestNumber 4
```
<img src="https://raw.githubusercontent.com/Nisha318/Nisha318.github.io/master/assets/images/thm/advent-of-cyber/2024/day4-20.png" alt="day4-22"><br>

## Questions
What was the flag found in the .txt file that is found in the same directory as the PhishingAttachment.xslm artefact?
- THM{GlitchTestingForSpearphishing}
What ATT&CK technique ID would be our point of interest?
- T1059
What ATT&CK subtechnique ID focuses on the Windows Command Shell?
- T1059.003
What is the name of the Atomic Test to be simulated?
- Simulate BlackByte Ransomware Print Bombing
What is the name of the file used in the test?
- Wareville_Ransomware.txt
What is the flag found from this Atomic Test?
- THM{R2xpdGNoIGlzIG5vdCB0aGUgZW5lbXk=}








 
