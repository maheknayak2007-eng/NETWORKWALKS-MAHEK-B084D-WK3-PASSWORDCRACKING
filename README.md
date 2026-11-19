# NETWORKWALKS-MAHEK-B084D-WK3-PASSWORDCRACKING (JTR + Networkwalks Tools)

This week had two mandatory modules, both cracking the password of the
same locked PDF (My Locked PDF1.pdf) but with different tools.

## PM1 - Password Cracking with JTR (John the Ripper + Johnny)

Used John the Ripper and the Johnny GUI on Windows to recover the
password of the protected PDF.

Steps:
1. Installed John the Ripper and Johnny, pointed Johnny to john.exe
2. Extracted the PDF's hash using an online pdf2john tool
3. Saved the hash to a text file and opened it in Johnny
4. Ran the attack - password cracked
5. Opened the PDF with the cracked password and got the flag

Cracked password: password1
Flag: nw{cybersecurity_flag_captured_2608}

Screenshots: see PM1-JTR-Johnny/screenshots/

## PM2 - Password Cracking with Networkwalks Tools

Did the same thing but using Networkwalks' own browser-based Hash
Calculator and Password Cracker instead of installing JTR.

Steps:
1. Uploaded the locked PDF to the Hash Calculator to extract the hash
2. Pasted the hash into the Password Cracker
3. Ran the dictionary attack - password cracked
4. Opened the PDF with the cracked password and got the flag

Cracked password: password1
Flag: nw{cybersecurity_flag_captured_2608}

Screenshots: see PM2-Networkwalks-Tools/screenshots/

## Notes

Both tools arrived at the same password for the same file, which makes
sense since they're both just running a dictionary attack against the
same PDF hash - JTR does it locally, Networkwalks' tool does it in the
browser.
