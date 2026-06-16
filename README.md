**NOTE:** If you are using Windows, please install **Windows Subsystem for Linux (WSL)** before the CTF. Many of the tools used throughout the challenges are command-line utilities designed for Linux environments and are most easily used through a Linux terminal.


# Steganography

## What is Steganography?

Steganography is a branch of cybersecurity where data is hidden inside another file. The embedded file and the cover file may or may not share the same format.

## Tools

* zsteg
* binwalk
* strings
* steghide
* Audacity
* 7-Zip
* WinRAR

## Tool Explanations

### Steghide

Used to extract hidden data from images without manually inspecting their binary contents.

### Binwalk

Used to identify and extract hidden files or data embedded within binaries.

### Strings

Sometimes the information you need is simply hidden as plaintext within a file's binary data. `strings` extracts all readable text from a file, making such data easier to find.

### 7-Zip and WinRAR

Used to create, open, and extract compressed archives such as `.zip` files.

### Zsteg

Similar to Steghide, but specifically useful for extracting data hidden within different color channels of an image.

# Crypto

## What is Cryptography?

At its simplest, cryptography is the practice of hiding information (primarily text) by converting it into data that appears meaningless or unreadable. The methods used to achieve this are called cryptographic techniques.

## Tools

* cyberchef.org
* dcode.fr

## Tool Explanations

### CyberChef and dCode

The Swiss Army knives of cryptography. They support a wide variety of encoding, decoding, encryption, decryption, and other cryptographic operations that you'll commonly encounter in CTF challenges.

# OSINT

## What is OSINT?

OSINT stands for **Open Source Intelligence**. In simple terms, it's the process of gathering information from publicly available sources. Think of it as following someone's public social media activity—one post can lead to another clue, eventually revealing information that wasn't immediately obvious.

## Tools

* Instagram
* Discord
* Reddit
* Internet Archive
* Google Lens
* Google Maps

## Tool Explanations

Most of these tools are fairly self-explanatory and are commonly used to gather, verify, and connect publicly available information.

# Network Security

# Web Exploitation

## What is Web Exploitation?

Ever opened **Inspect Element** and modified a webpage by adding or removing HTML elements? That's a very basic form of web exploitation. Web exploitation involves understanding how web applications work and identifying weaknesses in their implementation.

## Tools / Interfaces

Inside the browser's developer tools:

* Console
* Sources
* Network
* Application

## Tool Explanations

### Console

Used to execute JavaScript directly on the website.

### Sources

Contains the website's files, such as `index.html`, `styles.css`, and `script.js`.

### Network

Tracks the requests sent by the browser and the responses returned by the server.

### Application

Often contains stored data such as cookies, local storage, and authentication-related information.

# Reverse Engineering
