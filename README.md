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
<img width="1886" height="877" alt="Screenshot 2026-08-24 085408" src="https://github.com/user-attachments/assets/0cb84f4c-1f47-432b-8e38-baf8282648c9" />

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

<img width="1687" height="925" alt="Screenshot 2026-08-24 085707" src="https://github.com/user-attachments/assets/99644df6-f48d-43f6-b3b3-cf81496ea409" />


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

<img width="1726" height="890" alt="Screenshot 2026-08-24 085818" src="https://github.com/user-attachments/assets/306ff179-6126-42a1-9205-dc6d0bca6290" />

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
<img width="1740" height="899" alt="Screenshot 2026-08-24 085905" src="https://github.com/user-attachments/assets/876207ab-f78b-4933-b7f5-b9b6712da4a2" />

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
<img width="1377" height="868" alt="Screenshot 2026-08-24 091554" src="https://github.com/user-attachments/assets/8f8efcd1-8fa8-4082-919c-8fe692d24e4a" />

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
<img width="1270" height="865" alt="Screenshot 2026-08-24 091437" src="https://github.com/user-attachments/assets/7b7878ee-5831-4caf-9637-2e9ebb3bc01a" />

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
<img width="1872" height="916" alt="last" src="https://github.com/user-attachments/assets/c8a278cc-9243-473c-93f7-41a31b931c38" />

 
#DNS Enumeration



##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:



<img width="791" height="692" alt="image" src="https://github.com/user-attachments/assets/21dbc620-0bd4-4472-b73d-75e5a1bdda48" />




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
<img width="798" height="705" alt="image" src="https://github.com/user-attachments/assets/43719592-8c73-4293-b5d3-2ca425979936" />

<img width="803" height="707" alt="image" src="https://github.com/user-attachments/assets/ccaf8dbd-3edf-499f-9c7b-baae9a8f7862" />

<img width="792" height="710" alt="image" src="https://github.com/user-attachments/assets/395ef444-8e7c-4145-9652-59f0eb775e8e" />

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
<img width="952" height="727" alt="image" src="https://github.com/user-attachments/assets/91f605d3-a1b4-4292-b207-ebd4cf5b6f1e" />


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  
  
<img width="986" height="723" alt="image" src="https://github.com/user-attachments/assets/a3b5b41f-c6ae-4998-98a2-539e46077672" />

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

<img width="975" height="655" alt="image" src="https://github.com/user-attachments/assets/d6167619-9e65-4dd0-9d63-565bd9eef17e" />

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

