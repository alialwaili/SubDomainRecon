# SubDomainRecon  
*Comprehensive Subdomain Finder for Oman & GCC Regions*


## 📌 Features  
- Certificate Transparency (crt.sh) Lookup  
- DNS Zone Transfer Detection  
- Multi-threaded Brute-force (100 workers)  
- Oman/GCC-optimized Patterns  
- Smart Result Filtering  
- Custom Wordlist Support  

## 🚀 Quick Start  
```bash  
# Install dependencies  
pip install requests dnspython  

# Basic scan  
python subdomain.py example.com  

# Full scan with wordlist  
python subdomain.py oman.om -w wordlist1.txt  

📂 Wordlist Guidance
Included: wordlist1.txt (Basic 500 entries)
For Best Results:

Use Oman-specific wordlist (3000+ local terms)

Combine with Seclists DNS list

Add industry-specific terms (banking/energy)

⚠ Legal Requirements
Omani Law Compliance:

Requires written permission for .om domains

Avoid government domains (.gov.om)

Never scan banking (.bank.om) or critical infrastructure

🔍 Usage Tips
Timing: Scan 8PM-6AM GST for minimal impact

Validation:

bash
Copy
dig CNAME api.oman.om  
nslookup dev.oman.om  
Output: Save results with > oman_subs.txt

🌟 Sample Report
Copy
[*] Scanning oman.om...  
[+] crt.sh Found: 28 subdomains  
[!] Zone Transfer: Failed (NS01.oman.om)  
[*] Brute-forcing: 2915/3000 candidates  
[+] Total Unique Subdomains: 47  

admin.oman.om        eGov.oman.om  
rop-portal.oman.om   muscat-api.oman.om  
🛣 Development Roadmap
Arabic domain support (Punycode)

Omani CERT integration

GCC TLD priority system

Ramadan scanning schedule

📬 Contact
For Omani security collaboration:
Email: alialwaili@proton.me
