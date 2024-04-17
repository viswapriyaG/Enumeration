# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
![site](https://github.com/viswapriyaG/Enumeration/assets/131427787/bf9385b7-303a-42e5-968f-5440fc5801f4)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
![filetype](https://github.com/viswapriyaG/Enumeration/assets/131427787/3e58d06a-eaf9-4e88-8450-ea546b87e0aa)



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![intext](https://github.com/viswapriyaG/Enumeration/assets/131427787/f4a72cc7-c070-4cff-ab80-c6e744277226)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![inurl](https://github.com/viswapriyaG/Enumeration/assets/131427787/65948ddb-6394-4d00-a0eb-bfbab1d60019)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![intitle](https://github.com/viswapriyaG/Enumeration/assets/131427787/9b330ab0-1bf5-4676-abbf-63f51b663dfe)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![link](https://github.com/viswapriyaG/Enumeration/assets/131427787/d4306b94-e382-4575-a142-79c9ba354d34)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![cache](https://github.com/viswapriyaG/Enumeration/assets/131427787/228b9eb9-a9bf-4d06-8a10-1cd902875f69)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
![dns](https://github.com/viswapriyaG/Enumeration/assets/131427787/9daa1c59-f9b5-4e00-9c0b-42ed5cef0526)


##dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
![dnsenum](https://github.com/viswapriyaG/Enumeration/assets/131427787/56f0bb3f-2bf2-4b7c-9f80-5759a26c2965)
![dnsenum2](https://github.com/viswapriyaG/Enumeration/assets/131427787/fd36bb61-f64d-4790-b159-5f3ca4f52fc2)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same
![smtp](https://github.com/viswapriyaG/Enumeration/assets/131427787/e09061bb-69de-4215-820d-4e5e8102c2d6)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
![telnet](https://github.com/viswapriyaG/Enumeration/assets/131427787/5b646566-b6c4-429b-908c-87ebbe126f46)



## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.
![nmap smtp](https://github.com/viswapriyaG/Enumeration/assets/131427787/0ba4fa07-ae95-495e-ba17-cd6820eeacde)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

