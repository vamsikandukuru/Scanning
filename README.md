# Cybersecurity Internship Task 1 
## Scanning the local network for open ports using Nmap
## Tools used:
- Nmap
- xsltproc
  
## Steps
1. Find out the local IP range and host up or down.
2. Run a TCP SYN scan using NMAP.
3. Run aggresive scan for advanced scanning
4. Run NSE scripts for finding vulnerability
5. Save the scan output in .xml
6. Convert the .xml into HTML report.
   
## command
1. nmap -sS -A --script=vuln 192.168.0.0/24 -oX scan.xml.
2. xsltproc scan.xml -o scan.html

-sS - Syn scan.
-A  - Aggresive scan.
--script=vuln - for finding vulnerabilites on services running on the target ports.
-oX - for XML format.
-xsltproc - used to convert the .xml file into .html

## Files 
- 'scan.html' - Human-readale HTML generated from XML.



  

