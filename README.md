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
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/4ec3a51a-5cb2-4736-b384-7362b720fbac)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

## OUTPUT:
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/48a6728a-54ba-4f59-aea7-b28d33e2a201)

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

## OUTPUT:
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/5fd8c3a5-a87e-4451-b61b-27e8b3f2c5d5)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

## OUTPUT:
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/9d33fa57-ac37-4752-af71-5ea318355752)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

## OUTPUT:
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/a4fdda6b-db19-4d07-9121-e30c43047efb)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

## OUTPUT:
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/5ed6651b-ec2c-4f30-84f7-aeb9a737c1f6)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

## OUTPUT:
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/1d5aa82b-a816-4594-88df-adc8c6cb22c0)

## DNS Enumeration
## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/058c7fdc-a102-4452-8fe2-7fbff663fe91)
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/b17defd4-a540-4b00-b8fd-a5a463d75077)

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

## OUTPUT:
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/5d7653d2-1f75-4ef5-a884-b6489f8cf491)

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/c317071e-9c8f-4dd3-b766-7135c635e907)

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/eb9ef4c5-260f-4575-a632-6c3542b30cec)

select any username in the first column of the above file and check the same
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/59426147-2259-4a52-83e0-d20a7668e368)

## Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands

## OUTPUT:
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/965ecfac-ef10-4760-a770-ea5d7a25e540)

## nmap –script smtp-enum-users.nse <hostname>
The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:
![image](https://github.com/Harshinisrini1910/Enumeration/assets/161415847/20038e95-439f-4f35-8600-30b56c6e32c5)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully
