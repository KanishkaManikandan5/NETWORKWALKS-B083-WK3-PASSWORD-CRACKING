# NETWORKWALKS-B083-WK3-PASSWORD-CRACKING

## 📌 Overview
**Password cracking** is a cybersecurity technique used to recover or test the strength of passwords by systematically trying possible passwords through methods such as dictionary attacks, brute-force attacks, and password-guessing techniques. It is commonly used in authorized security testing to identify weak passwords and improve overall system security. This repository documents the **Week 3 Project Tasks**, focusing on **password cracking** of a protected PDF file using two different approaches:

1. **Module 1** – Password Cracking with **John the Ripper (JTR) & Johnny GUI**
2. **Module 2** – Password Cracking with **Networkwalks Hash Calculator & Password Cracker (online tools)**

Both tasks aim to recover the password protecting the same PDF file and demonstrate how weak passwords can be cracked quickly using dictionary-based attacks.

---

## 🎯 Objective
- Understand how password hashes are extracted from protected files.
- Learn how dictionary/wordlist-based password cracking works.
- Compare an offline tool (JTR + Johnny) with an online browser-based tool (Networkwalks Hash Calculator + Password Cracker).
- Reinforce why strong, complex passwords are essential for security.

---

## 🛠️ Tools Used

| Task | Tools |
|------|-------|
| Module 1 | John the Ripper (JTR), Johnny GUI, Online Hash Crack (PDF Hash Extractor) |
| Module 2 | Networkwalks Hash Calculator, Networkwalks Password Cracker |


---

## 📂 Module 1 — Password Cracking with JTR

### Steps
1. Downloaded **John the Ripper** and **Johnny GUI** from the official Openwall sources.
2. Installed Johnny and set the path to `john.exe` under Settings.
3. Extracted the PDF's crackable hash using the online PDF Hash Extractor tool (`pdf2john` equivalent).
4. Saved the extracted hash (starting with `$pdf$...`) into a text file (`hash1.txt`).
5. Opened the hash file in Johnny and clicked **Start new attack**.
6. Johnny successfully cracked the password.
7. Opened the PDF using the cracked password to confirm access.
---
## TASK 1 
TARGET : My-Locked-PDF1.pdf

![Purpose](https://github.com/KanishkaManikandan5/NETWORKWALKS-B083-WK3-PASSWORD-CRACKING/blob/040836f68badbe08612bb2a9c142fa44a7001a20/TASK%201.jpeg)


![Purpose](https://github.com/KanishkaManikandan5/NETWORKWALKS-B083-WK3-PASSWORD-CRACKING/blob/040836f68badbe08612bb2a9c142fa44a7001a20/TASK%201.1.jpeg)

![Purpose](https://github.com/KanishkaManikandan5/NETWORKWALKS-B083-WK3-PASSWORD-CRACKING/blob/040836f68badbe08612bb2a9c142fa44a7001a20/TASK%201.2.jpeg)

![Purpose](https://github.com/KanishkaManikandan5/NETWORKWALKS-B083-WK3-PASSWORD-CRACKING/blob/040836f68badbe08612bb2a9c142fa44a7001a20/TASK%201.3.jpeg)

---
## TASK 2
TARGET : My-Locked-PDF2.pdf

![Purpose](https://github.com/KanishkaManikandan5/NETWORKWALKS-B083-WK3-PASSWORD-CRACKING/blob/040836f68badbe08612bb2a9c142fa44a7001a20/TASK%202.jpeg)

![Purpose](https://github.com/KanishkaManikandan5/NETWORKWALKS-B083-WK3-PASSWORD-CRACKING/blob/040836f68badbe08612bb2a9c142fa44a7001a20/TASK%202.1.jpeg)

![Purpose](https://github.com/KanishkaManikandan5/NETWORKWALKS-B083-WK3-PASSWORD-CRACKING/blob/040836f68badbe08612bb2a9c142fa44a7001a20/TASK%202.3.jpeg)

---

## TASK 3
TARGET : My-Locked-PDF3.pdf

![Purpose](https://github.com/KanishkaManikandan5/NETWORKWALKS-B083-WK3-PASSWORD-CRACKING/blob/040836f68badbe08612bb2a9c142fa44a7001a20/TASK%203.jpeg)

![Purpose](https://github.com/KanishkaManikandan5/NETWORKWALKS-B083-WK3-PASSWORD-CRACKING/blob/040836f68badbe08612bb2a9c142fa44a7001a20/TASK%203.1.jpeg)

---

## 📂 Module 2 — Password Cracking with Networkwalks Tools

### Steps
1. Downloaded the locked PDF file (`My Locked PDF1.pdf`).
2. Opened the **Networkwalks Hash Calculator** and uploaded the PDF.
3. The tool extracted a hashcat/pdf2john-compatible hash (`$pdf$...`).
4. Copied the full hash value.
5. Opened the **Networkwalks Password Cracker** (dictionary attack tool).
6. Pasted the hash and ran the built-in wordlist attack (100 passwords).
7. The tool matched and displayed the cracked password.
8. Opened the PDF using the recovered password to confirm success.

### Result
![Purpose](https://github.com/KanishkaManikandan5/NETWORKWALKS-B083-WK3-PASSWORD-CRACKING/blob/38a76efbfae3f9535b8ac78fb2f4af5f036d81b8/TASK%204.jpeg)
![Purpose](https://github.com/KanishkaManikandan5/NETWORKWALKS-B083-WK3-PASSWORD-CRACKING/blob/38a76efbfae3f9535b8ac78fb2f4af5f036d81b8/TASK4.1.jpeg)
![Purpose](https://github.com/KanishkaManikandan5/NETWORKWALKS-B083-WK3-PASSWORD-CRACKING/blob/38a76efbfae3f9535b8ac78fb2f4af5f036d81b8/TASK%204.2.jpeg)

---

## 🔑 Key Learnings
- Password-protected files store passwords as **hashes**, not plaintext.
- Hashing is a **one-way function**; cracking relies on trying candidate passwords (dictionary/wordlist attacks) and comparing hashes, not reversing them.
- A short, common password like `password1` can be cracked within seconds/minutes.
- Both offline (JTR/Johnny) and online (Networkwalks) tools achieve the same result — the offline tool offers more flexibility (custom wordlists, rules), while the online tool is faster to set up with no installation.
- Strong passwords (12+ characters, mixed case, numbers, symbols) drastically increase cracking time and are essential for real-world protection.

---
# 👤 Author

**KANISHKA M**
Cybersecurity Intern B083

LinkedIn: <https://www.linkedin.com/in/kanishka-m525>
