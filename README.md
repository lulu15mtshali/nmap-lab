# Nmap Lab Report 
##Results 
- Port 135 (open) - Microsoft Windows RPC. Used for background system communications.
- Port 445 (open) - Microsoft Windows SMB. Used for Local file and printer sharing. 

##Conclusion
The scan completed successfully 



##Task 7: Vulnerability Scanning with Nikto 

I performed a Nikto vulnerability scan against the target server (testphp.vulnweb.com).

##Key Findings:
-**Server Software:** Running Apache/2.4.41 on Ubuntu.
-**Missing Security Headers:** The web application is missing vital anti-clickjaking ('X-Frame-options') and MIME-sniffing ('X-Content-Type-Options') headers.
-**Information Disclosure:** Discovered an exposed configuration backup file ('/config.php') and an exposed administrative path ('/admin/login.php').