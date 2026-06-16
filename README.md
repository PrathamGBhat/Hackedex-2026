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
* [dcode.fr](https://www.dcode.fr) - The Swiss Army knives of cryptography. They support a wide variety of hashing, encoding, decoding, encryption, decryption, and other cryptographic operations that you'll commonly encounter in CTF challenges.
* [crackstation.net](https://crackstation.net/) - Allows you to check pre computed hashes of commonly used passwords

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

### Tools

* [Wireshark](https://www.wireshark.org/download.html) -
* tshark (Ubuntu WSL - `sudo apt-get install wireshark tshark`) - 

## Web Exploitation

### What is Web Exploitation?

Ever opened **Inspect Element** and modified a webpage by adding or removing HTML elements? That's a very basic form of web exploitation. Web exploitation involves understanding how web applications work and identifying weaknesses in their implementation.

### Tools

Inside the browser's developer tools (inspect element):

* Console - Used to execute JavaScript directly on the website.
* Sources - Contains the website's files, such as `index.html`, `styles.css`, and `script.js`.
* Network - Tracks the requests sent by the browser and the responses returned by the server.
* Application - Often contains stored data such as cookies, local storage, and authentication-related information.

## Reverse Engineering

### What is Reverse Engineering?

### Tools
