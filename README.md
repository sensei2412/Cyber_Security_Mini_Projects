# Cyber_Security_Mini_Projects
A collection of 25 mini cybersecurity projects built to apply and reinforce concepts learned through TryHackMe, covering areas like network security, cryptography, web application security, penetration testing, and threat analysis. Each project translates theory into hands-on practice through small, focused, and well-documented implementations.

Projects
File Encryption & Decryption App (Sealbox): A browser app that encrypts and decrypts files with a password, entirely on your own device. It uses AES-256-GCM with a key derived through PBKDF2 (600,000 iterations), and even the original file name is hidden inside the encrypted data. Results can be saved as a simple .zip for sites that block unknown file types.

IP Address Information Finder: A Python command-line tool that looks up details about an IP address or a domain name, such as its location and network information. Private and reserved addresses are analysed offline, and there is a --json option for machine-readable output. It comes with a test suite.

Login Authentication System: A Java console app with registration, login and password change. Passwords are never stored in plain text but as salted PBKDF2-HMAC-SHA256 hashes, and an account is locked for five minutes after five failed attempts.

Network Port Scanner: A multi-threaded Python TCP scanner that finds open ports on a host and names the service behind each one. It supports port ranges, adjustable speed and timeouts, and optional banner grabbing. It should only be used on your own systems or ones you have permission to test

Password Generator: A browser tool that creates random passwords with the length and character types you choose. It can skip look-alike characters such as 0 and O, and it shows how strong the result is.

Password Strength Checker (Keystone): A browser tool that rates a password as you type and checks it against a list of requirements. It warns about personal details you want to avoid, flags reuse of another password, and can suggest a strong replacement.

Password Manager: A Python command-line vault that keeps all your logins in one encrypted file, locked with a master password that is never saved. The vault is protected with scrypt key derivation and AES-256-GCM, and the manager can generate secure passwords for new entries. It needs the cryptography package.

Phishing Website Detector (Phishing Link Inspector): A web page that inspects a link for common signs of phishing, such as brand names used on the wrong domain and other suspicious patterns. It knows commonly imitated brands, including Norwegian services like Vipps and BankID. Everything runs locally, so the link is never opened or sent anywhere.

Text Encryption (Caesar Cipher): A Python app that encrypts and decrypts text by shifting the letters of the alphabet. It has an interactive menu and command-line options, plus a brute-force mode that tries all 25 possible shifts to break a message.

Two-factor Authenticator: A Python app that generates the same 6-digit time-based codes (TOTP, RFC 6238) as Google Authenticator. You can add accounts, show live codes with a countdown, verify a code, and export an otpauth:// link for another app. It uses only the standard library.
URL Safety Checker: A tool that checks a web address for warning signs before you open it, such as odd domains, missing HTTPS and risky patterns. It gives a quick verdict from the text of the address alone, without visiting the link.
