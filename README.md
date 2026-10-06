# week-4-_Penetration-_Testing-_Black-_Box-_Report

![Kali Linux](https://img.shields.io/badge/Kali_Linux-Security-blue)
![John the Ripper](https://img.shields.io/badge/John_the_Ripper-Password_Cracking-purple)
![Target](https://img.shields.io/badge/Mediroza_General_Hospital-green)
![Type](https://img.shields.io/badge/Black_Box_PENTEST-blue)
![Ethical Hacking](https://img.shields.io/badge/Ethical_Hacking-Lab-red)

## Networkwalks Internship – Week 4 Project
Candidate: pavithra p

Internship Batch: sep26 Batch B083

Date: october 2026
## Executive Summary
A five-d ays black- b ox penetration test was conducted against the
external web infrastructure of Mediroza General Hospital. The assessment focused on identifying weaknesses in
the patient portal, authentication controls, protected patient documents, exposed server directories, andpublicly accessible 
databasebackups. The assessment identified a chained attack path beginning with information disclosure and authentication
weaknesses, followed by SQL injection, access to protected patientreports, weak PDF password protection, metadata disclosure,
and exposure of a database backup. The exposedbackup contained 3 confidential patient pathology reports, 30 confidential staffsalary information and 10 shareholder ownership data.

Overall Risk :CRITICAL

## TOOLS USED
|**TOOLS**|**PURPOSE**|
|---------|-----------|
| John the Ripper|To crack password|
| ExifTool|To get information about the report|
| Gobuster|	Directory Enumeration & Fuzzing	|
|Burp Suite|	Request Interception & Repeater |
| wget |grep	Remote File Retrieval & Parsing|
