# TryHackMe - Linux Fundamentals Part 1 Notes

## Task 1: Introduction  
_No answer needed_

---

## Task 2: A Bit of Background on Linux  
**Research:** What year was the first release of a Linux operating system?  
- **1991**

---

## Task 3: Interacting With Your First Linux Machine (In-Browser)  
I've deployed my first Linux machine!  
_No answer needed_

---

## Task 4: Running Your First Few Commands  

**Question:** If we wanted to output the text `"TryHackMe"`, what would our command be?  
- `echo "TryHackMe"`

<img src="/assets/linux/linux-fund1-1.png">

**Question:** What is the username of who you're logged in as on your deployed Linux machine?  
- **tryhackme**

<img src="/assets/linux/linux-fund1-2.png">

---

## Task 5: Interacting With the Filesystem  

**Question:** On the Linux machine that you deploy, how many folders are there?  
- **4**

<img src="/assets/linux/linux-fund1-3.png">

**Question:** Which directory contains a file?  
```bash
ls folder*
folder4
<img src="/assets/linux/linux-fund1-4.png">
Question: What is the contents of this file?

Hello World
<img src="/assets/linux/linux-fund1-5.png">
Question: Use the cd command to navigate to this file and find out the new current working directory. What is the path?

/home/tryhackme/folder4
<img src="/assets/linux/linux-fund1-6.png">
Task 6: Searching for Files
Question: Use grep on "access.log" to find the flag that has a prefix of "THM". What is the flag?
Answer format: ***{******}

THM{ACCESS}
<img src="/assets/linux/linux-fund1-7.png">
And I still haven't found what I'm looking for!
No answer needed

Task 7: An Introduction to Shell Operators
Question: If we wanted to run a command in the background, what operator would we want to use?

&
Question: If I wanted to replace the contents of a file named "passwords" with the word "password123", what would my command be?
Answer format: echo password123 > passwords

echo password123 > passwords

<img src="/assets/linux/linux-fund1-8.png">
Question: Now if I wanted to add "tryhackme" to this file named "passwords" but also keep "passwords123", what would my command be?
Answer format: **** ********* ** *********

echo tryhackme >> passwords
<img src="/assets/linux/linux-fund1-9.png">
Now use the deployed Linux machine to put these into practice.
No answer needed

Task 8: Conclusions & Summaries
I'll have a play around!
No answer needed

Task 9: Linux Fundamentals Part 2
Terminate the machine deployed in this room from Task 3.
No answer needed
