# News Headlines — Vulnerability Assessment Report </br>
**Author:** Varsha Asawale  
**Date:** 13-09-2025  
**Target:** Local lab (DVWA / OWASP Juice Shop)
## Executive Summary
- Tested in local lab environment (DVWA / Juice Shop)
- Findings: SQL Injection , Cross-Site Scripting , Insecure Authentication).
- All findings were exploited in lab and then fixed. Evidence and diffs are included.
## Scope & Tools
**Scope:** News Headlines web app (search, comments, headline create, admin login) in DVWA / Juice Shop lab.  
**Tools used:** Docker, Burp Suite (Proxy, Repeater, Intruder).

#  Finding 1 — SQL Injection
<img width="1525" height="954" alt="image" src="https://github.com/user-attachments/assets/01f31f8d-4480-4160-9390-7ca574fc64b2" />
### Evidence
<img width="1348" height="887" alt="image" src="https://github.com/user-attachments/assets/0eab0861-8985-47f9-9365-bbfee2f6c4be" />
<img width="1505" height="653" alt="image" src="https://github.com/user-attachments/assets/a40cc6da-be78-4a34-8836-5c9f3fbf664b" />
<img width="580" height="593" alt="image" src="https://github.com/user-attachments/assets/f98f3c4d-1fe0-430f-a248-4e32ef5f90dc" />
### Remediation
Replaced string-concatenated SQL with prepared statements (parametrized queries).
 # Finding 2 — Cross-Site Scripting
# XSS Reflected
<img width="1617" height="703" alt="image" src="https://github.com/user-attachments/assets/c1137364-04fe-4456-81f3-54a90be8e428" />
<img width="1393" height="883" alt="image" src="https://github.com/user-attachments/assets/aadd8dca-4092-42aa-acab-13c941dffe72" />
<img width="1079" height="392" alt="image" src="https://github.com/user-attachments/assets/81ee4aa0-07f6-4629-98c0-770eed5b3a31" />

#Stored XSS
<img width="1404" height="747" alt="image" src="https://github.com/user-attachments/assets/84a58b50-a78b-4448-8530-0c2bec4b1cec" />
<img width="1445" height="866" alt="image" src="https://github.com/user-attachments/assets/72850592-faad-4792-8c5e-e09406f41eb5" />
<img width="948" height="817" alt="image" src="https://github.com/user-attachments/assets/96637233-ddaf-4ce4-b5b5-0408f905a183" />
<img width="1140" height="426" alt="image" src="https://github.com/user-attachments/assets/c23f91c5-836f-46e1-af7f-87f8c4e18142" />




