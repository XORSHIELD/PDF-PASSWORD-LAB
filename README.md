<div align="center">

# 🔐 PDF PASSWORD AUDITING & RECOVERY LAB

### John the Ripper • pdf2john • RockYou • QPDF • Kali Linux

<img src="https://img.shields.io/badge/CYBERSECURITY-NETWORKWALKS-0A66C2?style=for-the-badge" />
<img src="https://img.shields.io/badge/WEEK%203-B083-6F42C1?style=for-the-badge" />
<img src="https://img.shields.io/badge/STATUS-COMPLETED-22C55E?style=for-the-badge" />
<img src="https://img.shields.io/badge/AUTHORIZED-YES-22C55E?style=for-the-badge" />

<br>

<img src="https://img.shields.io/badge/Kali%20Linux-2026-E87500?style=flat-square&logo=kalilinux&logoColor=white" />
<img src="https://img.shields.io/badge/John%20the%20Ripper-Password%20Auditing-C00000?style=flat-square" />
<img src="https://img.shields.io/badge/pdf2john-Hash%20Extraction-0070C0?style=flat-square" />
<img src="https://img.shields.io/badge/RockYou-Wordlist-238F89?style=flat-square" />
<img src="https://img.shields.io/badge/QPDF-PDF%20Decryption-E87500?style=flat-square" />

<br><br>
<!-- ===================== TYPING SVG ========================= -->

<p align="center">
  <img
    src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=600&size=24&duration=2500&pause=1000&color=39FF14&center=true&vCenter=true&width=900&lines=PDF+Security+Auditing;John+the+Ripper;Password+Hash+Analysis;Dictionary+Based+Password+Auditing;Kali+Linux+Security+Lab;QPDF+Document+Decryption;Cybersecurity+Practical;Ethical+Hacking"
    alt="Cybersecurity PDF password auditing and ethical hacking"
  />
</p>

**W3-PDF-PASSWORD-LAB | CYBERSECURITY | NETWORKWALKS**

### 👤 Danjuma Yusuf Joseph

**Cybersecurity Professional | Networkwalks Intern | Batch B083**

</div>
<img width="1690" height="913" alt="1-screenshot" src="https://github.com/user-attachments/assets/81ca1b17-4781-48e3-a89c-e5c0c457e708" />

---

# 🛡️ 1. Engagement Overview

| **Category** | **Details** |
|---|---|
| 👤 **Security Analyst** | Danjuma Yusuf Joseph |
| 🎓 **Program / Batch** | Networkwalks / B083 |
| 📅 **Assessment Period** | September 2026 |
| 🧪 **Lab Type** | Authorized Cybersecurity Training Lab |
| 🎯 **Primary Objective** | Audit and recover passwords from three password-protected PDF files |
| 🔐 **Primary Tool** | John the Ripper |
| 📄 **Hash Extraction** | pdf2john |
| 📚 **Wordlist** | RockYou |
| 🔓 **PDF Decryption** | QPDF |
| 🐉 **Operating System** | Kali Linux |
| 📁 **Targets** | My-Locked-PDF1.pdf, My-Locked-PDF2.pdf, My-Locked-PDF3.pdf |
| ✅ **Result** | 3/3 passwords recovered and PDFs decrypted |

---

# ⚠️ 2. Liability & Authorization Disclaimer

> **AUTHORIZED SECURITY TESTING ONLY**

This practical exercise was performed in an authorized cybersecurity training environment using PDF files supplied for password-auditing and learning purposes.

The techniques documented here must only be used against files, systems, accounts, or resources for which explicit authorization has been obtained.

Unauthorized password recovery or attempts to bypass access controls may violate applicable laws, regulations, organizational policies, or terms of service.

> 🛡️ **Security principle:** Always define and respect the authorized scope before performing password auditing or security testing.

---

# 🛡️ 3. Introduction

This practical exercise focused on **PDF password auditing and password recovery using John the Ripper on Kali Linux**.

The objective was to process three password-protected PDF documents, extract password-related hash information, perform a controlled dictionary-based password audit, identify the recovered passwords, and use the recovered credentials to decrypt copies of the original PDF files.

The three supplied targets were:

```text
My-Locked-PDF1.pdf
My-Locked-PDF2.pdf
My-Locked-PDF3.pdf

The assessment followed this workflow:

``` text
Password-Protected PDF
        ↓
     pdf2john
        ↓
John-Compatible Hash
        ↓
 John the Ripper
        ↓
  RockYou Wordlist
        ↓
 Recovered Password
        ↓
      QPDF
        ↓
 Decrypted PDF
        ↓
     Verification
```

Each activity was documented with:

-   🖥️ Command/tool used
-   📊 Observed result
-   📸 Supporting evidence
-   🔎 Security relevance
-   🛡️ Security recommendations
-   📝 Learning outcome

------------------------------------------------------------------------

# 🛠️ 4. Tools & Technologies

  -----------------------------------------------------------------------
  **Tool / Technology**               **Purpose**
  ----------------------------------- -----------------------------------
  🐉 **Kali Linux**                   Security testing and
                                      password-auditing environment

  🔐 **John the Ripper**              Password auditing and recovery

  📄 **pdf2john**                     Extracts PDF password information
                                      into John-compatible format

  📚 **RockYou**                      Dictionary/wordlist used for
                                      password candidate testing

  🔓 **QPDF**                         Uses the recovered password to
                                      create a decrypted PDF copy

  🖥️ **Terminal**                     Command execution and evidence
                                      collection
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# 🧪 5. Assessment Methodology

The assessment was divided into four stages.

## Phase 1 --- Target Identification

The three password-protected PDFs were identified and handled
individually.

## Phase 2 --- Hash Extraction

`pdf2john` was used to extract password-related information from each
PDF and save it to a separate hash file.

## Phase 3 --- Password Auditing

John the Ripper was executed against each extracted hash using the
RockYou wordlist.

## Phase 4 --- Password Verification & Decryption

The `john --show` command was used to display recovered passwords. QPDF
was then used with each recovered password to create a decrypted PDF
copy.

------------------------------------------------------------------------

# 📂 6. Target Files

The following files were assessed:

``` text
My-Locked-PDF1.pdf
My-Locked-PDF2.pdf
My-Locked-PDF3.pdf
```

Each target was processed independently.

------------------------------------------------------------------------

# 🔎 7. Activities Performed

## 7.1 🔐 PDF 1 --- Password Auditing

### Target

``` text
My-Locked-PDF1.pdf
```

### Step 1 --- Extract Password Hash

``` bash
pdf2john My-Locked-PDF1.pdf > hash1.txt
```

The extracted data was stored in:

``` text
hash1.txt
```

The hash could be reviewed with:

``` bash
cat hash1.txt
```

### Step 2 --- Run John the Ripper

``` bash
john --wordlist=/usr/share/wordlists/rockyou.txt hash1.txt
```

### Step 3 --- Display the Recovered Password

``` bash
john --show hash1.txt
```

### Observed Result

``` text
My-Locked-PDF1.pdf:good-luck
```

### Recovered Password

``` text
good-luck
```

### Step 4 --- Decrypt the PDF

``` bash
qpdf --decrypt --password='good-luck' My-Locked-PDF1.pdf output1.pdf
```

### Output

``` text
output1.pdf
```

The decrypted PDF was then opened to verify successful recovery.

------------------------------------------------------------------------

## 7.2 🔐 PDF 2 --- Password Auditing

### Target

``` text
My-Locked-PDF2.pdf
```

### Step 1 --- Extract Password Hash

``` bash
pdf2john My-Locked-PDF2.pdf > hash2.txt
```

### Step 2 --- Run John the Ripper

``` bash
john --wordlist=/usr/share/wordlists/rockyou.txt hash2.txt
```

### Step 3 --- Display the Recovered Password

``` bash
john --show hash2.txt
```

### Observed Result

``` text
My-Locked-PDF2.pdf:password1
```

### Recovered Password

``` text
password1
```

### Step 4 --- Decrypt the PDF

``` bash
qpdf --decrypt --password='password1' My-Locked-PDF2.pdf output2.pdf
```

### Output

``` text
output2.pdf
```

The decrypted PDF was opened to verify successful recovery.

------------------------------------------------------------------------

## 7.3 🔐 PDF 3 --- Password Auditing

### Target

``` text
My-Locked-PDF3.pdf
```

### Step 1 --- Extract Password Hash

``` bash
pdf2john My-Locked-PDF3.pdf > hash3.txt
```

### Step 2 --- Run John the Ripper

``` bash
john --wordlist=/usr/share/wordlists/rockyou.txt hash3.txt
```

### Step 3 --- Display the Recovered Password

``` bash
john --show hash3.txt
```

### Observed Result

``` text
My-Locked-PDF3.pdf:1qaz2wsx
```

### Recovered Password

``` text
1qaz2wsx
```

### Step 4 --- Decrypt the PDF

``` bash
qpdf --decrypt --password='1qaz2wsx' My-Locked-PDF3.pdf output3.pdf
```

### Output

``` text
output3.pdf
```

The decrypted PDF was opened to verify successful recovery.

------------------------------------------------------------------------

# 📊 8. Assessment Results

  ---------------------------------------------------------------------------------------------
              \# Target PDF             Hash File     Recovered     Decrypted       Status
                                                      Password      Output          
  -------------- ---------------------- ------------- ------------- --------------- -----------
               1 `My-Locked-PDF1.pdf`   `hash1.txt`   `good-luck`   `output1.pdf`   ✅
                                                                                    Completed

               2 `My-Locked-PDF2.pdf`   `hash2.txt`   `password1`   `output2.pdf`   ✅
                                                                                    Completed

               3 `My-Locked-PDF3.pdf`   `hash3.txt`   `1qaz2wsx`    `output3.pdf`   ✅
                                                                                    Completed
  ---------------------------------------------------------------------------------------------

### Overall Assessment

``` text
TARGETS TESTED
████████████████████ 3/3

PASSWORDS RECOVERED
████████████████████ 3/3

PDFs DECRYPTED
████████████████████ 3/3

RECOVERY SUCCESS
████████████████████ 100%
```

------------------------------------------------------------------------

# 🧠 9. Understanding the Commands

## `pdf2john`

``` bash
pdf2john My-Locked-PDF1.pdf > hash1.txt
```

`pdf2john` extracts the password-related information required by John
the Ripper from a protected PDF.

The `>` operator redirects the output into a text file.

------------------------------------------------------------------------

## `john`

``` bash
john --wordlist=/usr/share/wordlists/rockyou.txt hash1.txt
```

John the Ripper uses the supplied wordlist to test password candidates
against the extracted PDF password hash.

The same process was repeated for all three targets.

------------------------------------------------------------------------

## `john --show`

``` bash
john --show hash1.txt
```

This displays passwords that John the Ripper has successfully recovered
from the corresponding hash file.

------------------------------------------------------------------------

## `qpdf`

``` bash
qpdf --decrypt --password='good-luck' My-Locked-PDF1.pdf output1.pdf
```

QPDF uses the recovered password to create an accessible decrypted copy
of the protected PDF.

The original encrypted PDF remains unchanged.

------------------------------------------------------------------------

# 🧾 10. Evidence Collected

Evidence was collected throughout the practical exercise to demonstrate
the complete workflow from hash extraction through password recovery and
PDF decryption.



## 10.1 🔓 Evidence --- PDF 1 Password Recovery

The second evidence item demonstrates that John the Ripper successfully
recovered the password.

<img width="1683" height="903" alt="2-screenshot-pdf1" src="https://github.com/user-attachments/assets/6fab1fd4-d425-4090-8843-2de604ebee7b" />


------------------------------------------------------------------------

# 10.2 🔓 Evidence --- PDF 2 Password Recovery

The evidence demonstrates that John the Ripper successfully recovered
the password for the second target.

<img width="1684" height="911" alt="3-screenshot-pdf2" src="https://github.com/user-attachments/assets/7241d10d-b90f-47bc-b0d0-8aff73f51890" />


------------------------------------------------------------------------

# 10.3 🔓 Evidence --- PDF 3 Password Recovery

The evidence demonstrates successful recovery of the third PDF password.

<img width="1684" height="908" alt="4-screenshot-pdf3" src="https://github.com/user-attachments/assets/e6d588fb-7186-4e88-9092-5af33548d6d4" />



------------------------------------------------------------------------

# 🛡️ 11.  Security Recommendations

### 1. Use Strong and Unique Passwords

Avoid predictable words, common phrases, keyboard patterns, and
frequently reused passwords.

### 2. Prefer Long Passphrases

Long, unique passphrases increase the search space that an attacker
would need to test.

### 3. Avoid Password Reuse

Passwords protecting sensitive documents should not be reused across
other systems or accounts.

### 4. Protect Passwords Separately

When sending an encrypted document to another person, communicate the
password through a separate trusted channel.

### 5. Perform Authorized Password Audits

Organizations can periodically test password policies using controlled
security assessments.

### 6. Protect Sensitive Evidence

Recovered passwords, hashes, encrypted documents, and decrypted
documents should be treated as sensitive assessment material.

------------------------------------------------------------------------

# 🎓 12. Key Learning Outcomes

Through this practical exercise, I developed hands-on experience with:

-   🔐 PDF password auditing
-   🧩 Password hash extraction
-   🐉 John the Ripper
-   📄 pdf2john
-   📚 Dictionary-based password auditing
-   🔎 `john --show`
-   🔓 QPDF PDF decryption
-   🐉 Kali Linux command-line operations
-   📸 Security evidence collection
-   📝 Professional cybersecurity documentation
-   ⚖️ Authorized security-testing principles

The exercise demonstrated the relationship between:

``` text
Protected Document
        ↓
Hash Extraction
        ↓
Password Auditing
        ↓
Password Recovery
        ↓
Credential Verification
        ↓
PDF Decryption
        ↓
Evidence Collection
```

------------------------------------------------------------------------

# 📈 13. Assessment Progress

``` text
PHASE 1 — PDF Identification
████████████████████ 100% ✅

PHASE 2 — Hash Extraction
████████████████████ 100% ✅

PHASE 3 — Password Auditing
████████████████████ 100% ✅

PHASE 4 — Password Verification
████████████████████ 100% ✅

PHASE 5 — PDF Decryption
████████████████████ 100% ✅

PHASE 6 — Evidence Collection
████████████████████ 100% ✅

PHASE 7 — Documentation
████████████████████ 100% ✅
```

------------------------------------------------------------------------

# 🏆 14. Practical Results

``` text
TARGETS TESTED       3
HASHES EXTRACTED     3
PASSWORDS RECOVERED  3
PDFs DECRYPTED       3
SUCCESS RATE         100%
```

### Final Results

  Target                 Recovered Password   Result
  ---------------------- -------------------- --------------------------
  `My-Locked-PDF1.pdf`   `good-luck`          ✅ Recovered & decrypted
  `My-Locked-PDF2.pdf`   `password1`          ✅ Recovered & decrypted
  `My-Locked-PDF3.pdf`   `1qaz2wsx`           ✅ Recovered & decrypted

------------------------------------------------------------------------

# 📝 15. Conclusion

During this practical cybersecurity exercise, I performed an authorized
password-auditing assessment against three password-protected PDF
documents.

I used `pdf2john` to extract the password-related information required
by John the Ripper. I then used **John the Ripper with the RockYou
wordlist** to perform a controlled dictionary-based password audit.

After the passwords were recovered, I verified the results with
`john --show` and used **QPDF** to create decrypted copies of the three
PDF files.

The exercise demonstrated the complete workflow:

``` text
PDF Security
     ↓
Hash Extraction
     ↓
Password Auditing
     ↓
Password Recovery
     ↓
Credential Verification
     ↓
PDF Decryption
     ↓
Evidence Collection
```

The practical reinforced the importance of strong, unique, and
unpredictable passwords when protecting sensitive documents.

It also strengthened my practical understanding of **Kali Linux, John
the Ripper, pdf2john, RockYou, QPDF, password auditing, evidence
collection, and professional cybersecurity reporting**.

Most importantly, the exercise reinforced that password auditing and
security testing must always be performed within an **authorized
scope**.

> 🛡️ **Security principle: Strong security begins with strong
> credentials and controlled security testing.**

------------------------------------------------------------------------

## 16 👤 Author

**Danjuma Yusuf Joseph (XorShield)**

Cybersecurity Professional `B082`

LinkedIn: https://www.linkedin.com/in/xorshield/

## 📌 Project Information

**Program Name:** XorShield Home Lab | **Week:** 01 | **Project:** Cybersecurity & Pentesting Lab Setup | **Repository:** GitHub



------------------------------------------------------------------------

# 📌 17. Project Information

  **Project Detail**         **Information**
  -------------------------- ------------------------------------
  🏢 **Program**             Networkwalks Cybersecurity Program
  📅 **Week**                Week 03
  🎓 **Batch**               B083
  🔐 **Project Type**        Authorized Password Auditing Lab
  🎯 **Focus**               PDF Password Recovery
  🐉 **Primary OS**          Kali Linux
  🛠️ **Primary Tool**        John the Ripper
  📄 **Hash Extraction**     pdf2john
  🔓 **Decryption**          QPDF
  📚 **Wordlist**            RockYou
  📊 **Assessment Status**   Completed
  📁 **Documentation**       README.md

------------------------------------------------------------------------


### 🛡️ CYBERSECURITY • ETHICAL HACKING • PASSWORD SECURITY

**Learn → Practice → Analyze → Secure**



*W3-PDF-PASSWORD-LAB \| Networkwalks \| B083 \| September 2026*

