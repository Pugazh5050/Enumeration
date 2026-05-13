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

## OUTPUT:

<img width="1473" height="1090" alt="Screenshot 2026-02-04 082205" src="https://github.com/user-attachments/assets/42ab6161-db6e-4235-b702-e215af3fa145" />


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

## OUTPUT:

<img width="1445" height="1093" alt="Screenshot 2026-02-04 082246" src="https://github.com/user-attachments/assets/57f6d2d0-c304-466e-a0b3-5c70d128bfe8" />




intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

## OUTPUT:

<img width="1219" height="1095" alt="Screenshot 2026-02-04 082336" src="https://github.com/user-attachments/assets/3ecd079e-c96f-48be-83b4-fa2ddaf5ec9f" />



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

## OUTPUT:

<img width="1052" height="1085" alt="Screenshot 2026-02-04 082716" src="https://github.com/user-attachments/assets/a4f4ba38-ffe4-45d8-a943-cb7b764f7b3d" />

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

## OUTPUT:

<img width="1185" height="1094" alt="Screenshot 2026-02-04 082951" src="https://github.com/user-attachments/assets/804c802d-4eae-4cc4-b302-f5d0cf971a66" />


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

## OUTPUT:

<img width="1179" height="1096" alt="Screenshot 2026-02-04 083027" src="https://github.com/user-attachments/assets/168b6eb0-f5f2-4f74-b6df-007d33e0e1b5" />


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

## OUTPUT:

<img width="1182" height="1090" alt="Screenshot 2026-02-04 083358" src="https://github.com/user-attachments/assets/c3af2385-c9d4-4d0f-bd0d-0935da5aba80" />


 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

## OUTPUT:


<img width="1543" height="619" alt="Screenshot 2026-02-04 092511" src="https://github.com/user-attachments/assets/a9273b6c-e382-45f4-a4e8-5e5fa3e5d0a6" />





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

## OUTPUT:

<img width="1384" height="689" alt="Screenshot 2026-02-04 092532" src="https://github.com/user-attachments/assets/cb81f614-82a2-42a5-966c-ced313a41d7e" />


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

## OUTPUT:

<img width="1126" height="390" alt="Screenshot 2026-02-04 092552" src="https://github.com/user-attachments/assets/d7070c0f-a036-442b-bb79-76d9a1dd1bed" />



#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output: 
 
 <img width="1713" height="543" alt="Screenshot 2026-02-04 092859" src="https://github.com/user-attachments/assets/cbf6671b-2734-4ba0-b3f2-347a13add275" />

  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
<img width="1293" height="393" alt="Screenshot 2026-02-04 092606" src="https://github.com/user-attachments/assets/d479e9ff-2052-4d4a-856d-3bce23ab203e" />


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

