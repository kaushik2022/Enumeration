# Ex03-Enumeration
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
---
**Google Hacking:**

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

**site:** This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com


**filetype:** This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

<img src="https://github.com/user-attachments/assets/8aa569ab-f3eb-4afa-8eb4-a70e72176060" width=50%>



**intext:** This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

<img src="https://github.com/user-attachments/assets/f1af0fb8-3b01-4d5f-913b-62b9b45f65a2" width=50%>


**inurl:** This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

<img src="https://github.com/user-attachments/assets/ab2305b2-b5fa-4b07-86ac-104645a9e254" width=50%>

**intitle:** This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

<img src="https://github.com/user-attachments/assets/807f99a5-a0c3-4066-8bc8-5557340a2975" width=50%>

**link:** This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

<img src="https://github.com/user-attachments/assets/093cafcd-974f-425d-8ca3-b6926c0161a9" width=50%>

**cache:** This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

<img src="https://github.com/user-attachments/assets/edc411e8-dd79-47a1-8046-2f39802cf4a9" width=50%>

---
 
# DNS Enumeration
<img src="https://github.com/user-attachments/assets/d3b49a5c-10db-495f-ad87-7227d7aa5fd0" width=50%>

---

## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

## OUTPUT:
<img src="https://github.com/user-attachments/assets/a3a6783a-2a4c-434f-9d61-a6d74ec427e9" width=50%>


---

## dnsenum
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

<img src="https://github.com/user-attachments/assets/0c9443fd-8e48-4c1d-82fb-7a0eb9d40883" width=50%>

---

## SMTP-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
<img src="https://github.com/user-attachments/assets/30f116d9-420c-4316-907a-4dce6f888bf9" width=50%>


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

<img src="https://github.com/user-attachments/assets/8e7482f4-aa8e-403f-9a71-a28198629067" width=50%>

Select any username in the first column of the above file and check the same

<img src="https://github.com/user-attachments/assets/417fbd94-ca6c-41fb-9164-3a83703c79d7" width=50%>

---
# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
 ![WhatsApp Image 2025-04-26 at 08 32 30_0612beb1](https://github.com/user-attachments/assets/286d90a2-2429-4125-bce3-3ee50130cd0e)
 
 ## Output
  
<img src="https://github.com/user-attachments/assets/66ff873f-f2f1-48be-aa5a-171f7bf1f9f8" width=50%>
 
---
## NMAP –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

<img src="https://github.com/user-attachments/assets/b5b70009-e9fd-4863-b8f8-e2b6652aed33" width=50%>


## OUTPUT:

<img src="https://github.com/user-attachments/assets/81238996-5f4a-4936-a30b-c3ad85579f64" width=50%>

---

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

