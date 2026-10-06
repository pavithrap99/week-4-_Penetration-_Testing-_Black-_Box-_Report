# week-4-_Penetration-_Testing-_Black-_Box-_Report

![Kali Linux](https://img.shields.io/badge/Kali_Linux-Security-blue)
![John the Ripper](https://img.shields.io/badge/John_the_Ripper-Password_Cracking-purple)
![Target](https://img.shields.io/badge/Mediroza_General_Hospital-green)
![Type](https://img.shields.io/badge/Black_Box_PENTEST-blue)
![Ethical Hacking](https://img.shields.io/badge/Ethical_Hacking-Lab-red)

## Networkwalks Internship – Week 4 Project
**Candidate**: pavithra p

**Internship Batch**: sep26 Batch B083

**Date**: october 2026
## Executive Summary
A five-d ays black- b ox penetration test was conducted against the
external web infrastructure of Mediroza General Hospital. The assessment focused on identifying weaknesses in
the patient portal, authentication controls, protected patient documents, exposed server directories, andpublicly accessible 
databasebackups. The assessment identified a chained attack path beginning with information disclosure and authentication
weaknesses, followed by SQL injection, access to protected patientreports, weak PDF password protection, metadata disclosure,
and exposure of a database backup. The exposedbackup contained 3 confidential patient pathology reports, 30 confidential staffsalary information and 10 shareholder ownership data.

Overall Risk :CRITICAL

## 🛠️ TOOLS USED
|**TOOLS**|**PURPOSE**|
|---------|-----------|
| John the Ripper|To crack password|
| ExifTool|To get information about the report|
| Gobuster|	Directory Enumeration & Fuzzing	|
|Burp Suite|	Request Interception & Repeater |
| wget |grep	Remote File Retrieval & Parsing|
## Testing Methodology

The assessment followed a black-box penetration testing approach:

1. Information gathering
2. File and metadata analysis
3. Password/hash analysis
4. Credential testing
5. Sensitive information identification
6. Security findings documentation
7. Recommendations

## 🔥 Key Findings & Data Exposure
|Identifier|	Vulnerability|	Severity	|Exploit Result|
|----------|---------------|-----------|--------------|
|01 |SQL Injection (Boolean-Based) |🔴 Critical|	Admin login bypass using admin' -- |
|02	|Weak Cryptographic Storage (PDF)|	🟠 High|	Decrypted 3 patient files with rockyou.txt|
|03 |	Directory Listing & Data Leak  |	🔴 Critical|	Exposed mediroza_db_backup_2019.sql|

## 📂 Exposed Data Breakdown
1. Patient Medical Records

* **Sipho Dlamini** (MG-P-10231) - Abnormal White Cell Count.

* **Priya Reddy** (MG-P-10244) - High Cholesterol & Triglycerides.

* **Emily Thompson** (MG-P-10258) - Iron Deficiency (Low Ferritin & Vitamin D).

2. Hospital Payroll (30 Employees)

 * The staff table exposed monthly salaries in ZAR. The highest salary was R160,000 (Medical Director), and the lowest was R19,000
    (Receptionist).

3. Shareholder Structure
   
 * Dr. Rajesh Naidoo holds a 18.0% majority stake, while Dr. Vikram Chetty holds a 4.0% Preferential share class.

 ##  ⭐ Project Status
|Milestone|	Objective|Status|
|---------|----------|--------|
|M1	|Breach & Retrieve 3 PDFs|✅ Complete|
|M2	|Crack Encryption & Extract Text|✅ Complete|
|M3|Find Salaries & Shareholders|✅ Complete|
|M4|Compile Professional Report	|✅ Complete|
|Final|	Portfolio & GitHub Documentation|✅ Complete|

 ##  ⚠️ Ethical & Legal Disclaimer
IMPORTANT This project was conducted strictly for educational purposes as part of the Networkwalks Internship Program (Batch B083 | Week 4). The target environment (https://medirozahospital.com) is a simulated training lab designed explicitly for cybersecurity education. Written authorization was granted by the training provider prior to testing.

The techniques and code demonstrated in this repository must never be applied to any system, network, or application without obtaining explicit, written permission from the rightful owner. Unauthorized access is illegal and unethical.

## Author
pavithra p

 [![LinkedIn](https://img.shields.io/badge/LinkedIn-Pavithra-blue?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/pavithra-p-202131427/)
 
[![GitHub](https://img.shields.io/badge/GitHub-Pavithra-black?logo=github&logoColor=purple)](https://github.com/pavithrap99)

Networkwalks Internship:Bacth-B083 Week-4
