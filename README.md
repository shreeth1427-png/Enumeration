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

<img width="1036" height="677" alt="Screenshot 2026-08-22 090250" src="https://github.com/user-attachments/assets/f6dff0ab-b2b0-40b7-a0f2-1fbd23e27293" />

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

<img width="1041" height="668" alt="Screenshot 2026-08-22 090304" src="https://github.com/user-attachments/assets/c7dc7b11-9356-4c6f-986c-44a13f2a6530" />


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
<img width="1033" height="686" alt="Screenshot 2026-08-22 090316" src="https://github.com/user-attachments/assets/ef3f6826-8702-473d-9e3b-576f1161ef97" />

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
<img width="1039" height="688" alt="Screenshot 2026-08-22 090330" src="https://github.com/user-attachments/assets/2dc27bde-2c58-42d3-97a1-3490af2fcfc3" />

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
<img width="1036" height="679" alt="Screenshot 2026-08-22 090344" src="https://github.com/user-attachments/assets/cda1d372-6677-4b66-b093-9d0f923de72b" />

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
<img width="1038" height="728" alt="Screenshot 2026-08-22 090355" src="https://github.com/user-attachments/assets/927fe54d-5844-4456-80ec-c2f19427e442" />

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
<img width="1036" height="685" alt="Screenshot 2026-08-22 090406" src="https://github.com/user-attachments/assets/0e7d0bbf-5bcd-4043-9ea6-d35b3198a23c" />
 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

<img width="985" height="755" alt="Screenshot 2026-08-22 090427" src="https://github.com/user-attachments/assets/1cf2bcc2-396e-4738-b7e5-0fa493f26a48" />

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
<img width="987" height="852" alt="Screenshot 2026-08-22 090458" src="https://github.com/user-attachments/assets/4375be28-8576-4641-b313-dcd9eba2fe6f" />
<img width="985" height="806" alt="Screenshot 2026-08-22 090521" src="https://github.com/user-attachments/assets/e5047a9e-dfaf-4e77-94e2-da612190cc89" />
<img width="978" height="801" alt="Screenshot 2026-08-22 090536" src="https://github.com/user-attachments/assets/e6f206d6-8e6d-4c21-8e06-2f6ec7c91462" />
<img width="1040" height="783" alt="Screenshot 2026-08-22 090549" src="https://github.com/user-attachments/assets/d3f1c840-b781-4906-8576-4848429a1d55" />

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  
 <img width="1028" height="754" alt="Screenshot 2026-08-22 090601" src="https://github.com/user-attachments/assets/4f9457c2-fff1-43ed-99be-c62d1579c94d" />

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:
<img width="1041" height="703" alt="Screenshot 2026-08-22 090612" src="https://github.com/user-attachments/assets/416103a8-bbab-4441-a1ca-a0e851d62485" />

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

