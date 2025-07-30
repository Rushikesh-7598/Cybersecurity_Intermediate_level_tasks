# Cybersecurity_Intermediate_level_tasks

This repository highlights the intermediate level security tasks I performed during my cybersecurity internship at ShadowFox. Each task offered hands-on exposure to real-world attack techniques helping me understand how attackers operate and how defenders can stay one step ahead.

As part of this journey, I completed three key tasks: ->VeraCrypt Password Cracking & File Decryption ->Executable Entry Point Analysis ->Reverse Shell Exploitation using Metasploit

These challenges helped me build a solid foundation in ethical hacking and system exploitation. Task 1: VeraCrypt File Decryption Objective: To decode a hashed password and use it to unlock an encrypted VeraCrypt volume.

Tools Used: John the Ripper (Kali), VeraCrypt (Windows)

Summary: I was provided with a password hash stored in a file. I identified the hash type and cracked it using a password cracking tool. Once retrieved, I used the password in VeraCrypt on Windows to mount the encrypted volume and explore its contents.

Impact: Even the strongest encryption becomes vulnerable if weak or guessable passwords are used.

Mitigation: Enforce strong password policies and avoid storing unsalted hashes in plain text.

Task 2: Entry Point Analysis of Executable Objective: To identify where the execution of a Windows program begins by analyzing its binary structure.

Tools Used: PE-bear (Windows)

Summary: I loaded a Windows .exe file into PE-bear and explored its internal structure. I successfully located the address of the entry point the first instruction that runs when the executable is launched. This is a crucial concept in reverse engineering and malware analysis.

Impact: Understanding entry points can help detect injected malicious code and support deeper binary analysis.

Mitigation: Always inspect and verify executables before execution especially those from untrusted sources.

Task 3: Reverse Shell Exploitation Objective: To simulate an attack by gaining remote access to a Windows machine from Kali using a reverse shell.

Tools Used: Metasploit Framework, Msfvenom, Kali Linux, Windows 10 (VirtualBox)

Summary: I created a malicious payload, executed it on a Windows target and successfully established a reverse shell connection from my Kali machine. This exercise demonstrated how easily attackers can gain full control when social engineering or poor endpoint protection exists.

Impact: Reverse shells are powerful tools that allow attackers to manipulate a system remotely.

Mitigation: Use endpoint protection, avoid running unknown files and restrict outbound traffic using firewalls.

Conclusion: These tasks gave me real insight into the offensive side of cybersecurity. I didn’t just learn tools I learned how attackers think. This experience strengthened my skills in ethical hacking and helped me better appreciate the importance of layered defense.
