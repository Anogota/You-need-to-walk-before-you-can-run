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
