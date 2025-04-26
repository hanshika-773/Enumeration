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

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:







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


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
### site:example.com
![Screenshot 2025-04-26 062544](https://github.com/user-attachments/assets/292b8490-b899-4867-aa4c-146b0ad0dce1)
### filetype:pdf
![Screenshot 2025-04-26 062559](https://github.com/user-attachments/assets/122448cf-c8a8-44a5-8eab-d340670f5fd7)
### intext:password
![Screenshot 2025-04-26 062610](https://github.com/user-attachments/assets/41fac2d7-9457-41df-87e4-0ab6d94d641a)
### inurl:admin
![Screenshot 2025-04-26 062621](https://github.com/user-attachments/assets/5bc7f252-3d56-415b-bf58-dc1b022b30e9)
### intitle:index of
![Screenshot 2025-04-26 062633](https://github.com/user-attachments/assets/9f4e5aca-3fa7-4aaf-91c3-9f4445d29856)
### link:example.com
![Screenshot 2025-04-26 062643](https://github.com/user-attachments/assets/79ae0ff4-a103-42fa-b5ef-a1525cd191e7)
### cache:example.com
![Screenshot 2025-04-26 062653](https://github.com/user-attachments/assets/b952d195-6ef8-4305-ae19-60194d6ca036)
## DNS Enmueration
### DNS Recon
![Screenshot 2025-04-26 063043](https://github.com/user-attachments/assets/ab5b6559-6632-48ed-9dca-efca62885945)

### dnsenum
![Screenshot 2025-04-26 063057](https://github.com/user-attachments/assets/fdff18fd-8768-4417-a432-cdebe58d760d)

### smtp-user-enum
![Screenshot 2025-04-26 063109](https://github.com/user-attachments/assets/6cc6f9f7-83c4-4a7e-a447-1920860a5be9)
![Screenshot 2025-04-26 063122](https://github.com/user-attachments/assets/14efc5a4-e5dc-4589-b808-fdabdf6e456a)

### Telnet for smpt enumeration
![Screenshot 2025-04-26 063133](https://github.com/user-attachments/assets/799b145d-2824-450f-aac1-14df5e90506b)

### nmap-script smtp-enum-user.nse
![Screenshot 2025-04-26 063139](https://github.com/user-attachments/assets/a2ed28c9-93aa-44c4-8f1a-27bf100a7556)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

