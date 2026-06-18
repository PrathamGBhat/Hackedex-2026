# What is a CTF?
    
A Capture The Flag (CTF) is a gamified cybersecurity competition where participants have to uncover hidden strings of text called "flags" for points.
To obtain these hidden strings, the users have to apply real world cybersecurity techniques at a scaled down level.

# Rules and Regulations for Hackemon 2.0

*1. Reporting to the CTF*
- *Check your Alloted Venues*: Each team has been alloted one of three venues. Check them in the official WhatsApp group beforehand
- *Mark your Attendance*: Inform the volunteers at the entrance about your presence.

*2. General Conduct*
- *Respect All Participants*: Harassment or malicious behavior is prohibited. Treat everyone with respect.
- *Fair Play*: Play honestly. Exploiting platform vulnerabilities for an advantage leads to disqualification.

*3. Challenge Solving*
- *Own Work Only*: Solve challenges yourself. Plagiarism (using others' solutions or pre-made scripts) will result in disqualification.
- *Tools*: Any tools may be used, but automating challenge solutions (e.g., flag scrapers or brute-forcing) is not allowed.

*4. Communication and Collaboration*
- *Public Discussion*: Discussion of flags in general in public will lead to direct disqualification!
 
*5. Flag Submission*
- *Flag Format*: Flags must be submitted in the format: hackemon{...}. Case sensitivity matters.
- *One Flag, One Submission*: Each flag can be submitted only once. If incorrect, solve the challenge again for the correct flag.

*6. Exploiting System Vulnerabilities*
- *No Attacks on Platform*: Any attack or disruption of the CTF platform (e.g., DoS or SQL injection) will result in disqualification.
- *Use of Other Platforms*: Attacking external websites or systems that affect the event or your team's score will lead to disqualification.

*7. Offline CTF*
- *No Trespassing*: All the questions involve testing a set proximity to the location in riddle. Coding Club will not take responsibility in case of players entering buildings.

# Setup

If you are using Windows, please install [**Windows Subsystem for Linux (WSL)**](https://www.youtube.com/watch?v=9gT6vO_W6x0) before the CTF. Many of the tools used throughout the challenges are command-line utilities designed for Linux environments and are most easily used through a Linux terminal.

# Verticals of Cybersecurity

## Steganography

### What is Steganography?

Steganography is a branch of cybersecurity where data is hidden (embedded) inside another file. The embedded file and the cover file may or may not share the same format.

### Tools

* strings (Ubuntu WSL - `sudo apt update && sudo apt install binutils -y`) - Sometimes the information you need is simply hidden as plaintext within a file's binary data. `strings` extracts all readable text from a file, making such data easier to find.
* steghide (Ubuntu WSL - `sudo apt-get install steghide`) - Used to extract hidden data from images without manually inspecting their binary contents.
* zsteg (Ubuntu WSL - `sudo apt install ruby ruby-dev build-essential -y && sudo gem install zsteg`) - Similar to Steghide, but specifically useful for extracting data hidden within different color channels of an image.
* binwalk (Ubuntu WSL - `sudo apt-get install binwalk`) - Used to identify and extract hidden files or data embedded within binaries.
* [Audacity](https://www.audacityteam.org/download/) - Used to extract data from audio file spectograms
* [7-Zip](https://7-zip.org/download.html) - Used to create, open, and extract compressed archives such as `.zip` files.
* [WinRAR](https://www.rarlab.com/download.htm) - Alternate to 7-zip

## Crypto

### What is Cryptography?

At its simplest, cryptography is the practice of hiding information (primarily text) by converting it into data that appears meaningless or unreadable. The methods used to achieve this are called cryptographic techniques.

### Tools

* [cyberchef.org](https://www.cyberchef.org)
* [dcode.fr](https://www.dcode.fr)

The Swiss Army knives of cryptography. They support a wide variety of hashing, encoding, decoding, encryption, decryption, and other cryptographic operations that you'll commonly encounter in CTF challenges.

* [pentesterworld.com](https://pentesterworld.com/tools/hash-cracker) 
* [crackstation.net](https://crackstation.net/)

Both of these tools allow you to check pre computed hashes of commonly used passwords

## OSINT

### What is OSINT?

OSINT stands for **Open Source Intelligence**. In simple terms, it's the process of gathering information from publicly available sources. Think of it as following someone's public social media activity—one post can lead to another clue, eventually revealing information that wasn't immediately obvious.

### Tools

* Google Lens
* Google Maps
* [Instagram](https://www.instagram.com)
* [Discord](https://www.discord.com)
* [Reddit](https://www.reddit.com)
* [Internet Archive/Wayback Machine](https://archive.org/)

## Network Security

### What is Network Security?

Network security is the practice of protecting a computer network's infrastructure, traffic, and data from unauthorized access, misuse, modification, or cyberattacks.

### Tools

* [Wireshark](https://www.wireshark.org/download.html) - Tool that allows you to intercept, log, and inspect individual data packets for troubleshooting and analysis
* tshark (Ubuntu WSL - `sudo apt-get install wireshark tshark`) - Same functionality as wireshark but on the command line interface (CLI)

## Web Exploitation

### What is Web Exploitation?

Ever opened **Inspect Element** and modified a webpage by adding or removing HTML elements? That's a very basic form of web exploitation. Web exploitation involves understanding how web applications work and identifying weaknesses in their implementation.

### Tools

Inside the browser's developer tools (inspect element):

* Console - Used to execute JavaScript directly on the website.
* Sources - Contains the website's files, such as `index.html`, `styles.css` and `script.js`.
* Network - Tracks the requests sent by the browser and the responses returned by the server.
* Application - Often contains stored data such as cookies, local storage, and authentication-related information.

## Reverse Engineering

### What is Reverse Engineering?

Reverse engineering is the process of deconstructing a compiled software binary or hardware system to analyze its structure, functions, and logic to understand how it works without access to the original source code.

### Tools

* uncompyle6 (`pip install uncompyle6`)
* dis (In-built with python)
* decompyle3 (`pip install decompyle3`)
