# InformationGathering
Information Gathering Techiques

# To perform information gathering techniques

# AIM:

To perform information gathering techniques using kali linux 

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:
Open terminal/browser and try execute necessary commands/use url to perform information gathering

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified for information gathering:

Footprinting is a part of the reconnaissance process which is used for gathering possible information about a target computer system or network.
http://www.whois.com/whois website to get detailed information about a domain name information including its owner, its registrar, date of registration, expiry, name server, owner's contact information, etc.

## OUTPUT:
<img width="1905" height="901" alt="wois" src="https://github.com/user-attachments/assets/cb2aa03b-af00-40f1-a6f1-3fcf9d9e026c" />

### Explanation 
The `whois` command in Linux is used to obtain detailed information about a domain name, IP address, or website registration. It queries WHOIS databases maintained by domain registrars and internet authorities to display details such as domain owner information, registration date, expiration date, registrar name, DNS servers, and contact details if publicly available. This command is widely used by network administrators, cybersecurity professionals, and website owners for domain verification, security investigations, troubleshooting, and checking domain availability. It helps identify who manages a particular website or server on the internet. Example usage: `whois example.com`.


## Finding IP address:
ping command is available on Windows as well as on Linux OS. Following is the example to find out the IP address of facebook.com.
##output
<img width="649" height="238" alt="Screenshot_2026-04-30_04-34-28" src="https://github.com/user-attachments/assets/76974f7f-8536-4c29-ad21-fcf423571716" />

### Explanation 
`ping` is a Linux network diagnostic command used to check whether a device, server, or website is reachable over a network. It works by sending ICMP (Internet Control Message Protocol) echo request packets to a target IP address or domain name and waiting for a reply. The command also measures the response time, helping users identify network delays or connectivity issues. It is commonly used by system administrators, developers, and network engineers for troubleshooting internet connections, testing server availability, and verifying communication between devices in a LAN or the internet. Example usage: `ping google.com`.


## Finding Hosting Company
get further detail by using ip2location.com website.

## output

<img width="1754" height="851" alt="Screenshot_2026-04-30_04-37-59" src="https://github.com/user-attachments/assets/e11bd466-23cf-40b2-849d-7d9f0b5032b3" />

<img width="1754" height="851" alt="Screenshot_2026-04-30_04-37-59" src="https://github.com/user-attachments/assets/03fa17b8-e6cc-4c68-92ac-2dc596a2bede" />

### Explanation 
It is a website and online service that provides IP geolocation information. It helps users identify the approximate physical location of an IP address, including country, state, city, latitude, longitude, ISP (Internet Service Provider), timezone, ZIP code, and proxy or VPN usage details. The platform offers tools such as IP lookup, geolocation databases, APIs, and cybersecurity-related services for developers and businesses. It is commonly used in network security, fraud detection, website analytics, digital marketing, content localization, and access control systems. The service is widely used by developers and organizations needing location-based internet data.


## History of the website:
## output
https://web.archive.org/

<img width="1736" height="824" alt="Screenshot_2026-04-30_04-44-07" src="https://github.com/user-attachments/assets/fd4a0c7d-fae8-482f-87ba-d30eb50c6a79" />

<img width="1303" height="767" alt="Screenshot_2026-04-30_04-44-27" src="https://github.com/user-attachments/assets/4684afbb-9f26-4b1b-9089-ce6b9f4c529b" />

### Explanation 
The `web.archive.org` website, also known as the Wayback Machine, is an online digital archive that stores historical snapshots of websites and web pages from different time periods. It allows users to view older versions of websites, even if the original content has been changed or removed. The service is maintained by the Internet Archive and is widely used for research, cybersecurity investigations, academic references, legal evidence, and recovering deleted web content. Users can search a URL to see archived copies captured over many years. It helps preserve the history and evolution of the internet and publicly accessible websites.

# Webserver Fingerprinting:

## Netcat:
sudo nc example.com 80
GET / HTTP/1.1
Host: example.com


<img width="226" height="96" alt="Screenshot_2026-04-30_04-51-58" src="https://github.com/user-attachments/assets/9fc5e4db-06f3-4c4b-b8c0-17ab93827d15" />

### Explanation 
The `netcat` command, often called `nc`, is a powerful networking utility in Linux used for reading, writing, and transferring data across network connections using TCP or UDP protocols. It can function as a client or server and is widely used for network debugging, port scanning, file transfers, chat communication, and testing open ports or services. System administrators and cybersecurity professionals commonly use it for troubleshooting network services and creating simple communication channels between devices. Netcat is also useful in scripting and automation because of its flexibility. Example usage: `nc -zv example.com 80` checks whether port 80 is open on a server.


## nmap:

## output
<img width="913" height="240" alt="Screenshot_2026-04-30_04-49-39" src="https://github.com/user-attachments/assets/01382d56-51b0-453f-a787-63a1fd166350" />

### Explanation 
The `nmap` command, short for Network Mapper, is a Linux network scanning and security auditing tool used to discover devices, open ports, running services, operating systems, and potential vulnerabilities on a network. It sends specially crafted packets to target systems and analyzes their responses to gather network information. `nmap` is widely used by system administrators, ethical hackers, and cybersecurity professionals for network monitoring, penetration testing, vulnerability assessment, and troubleshooting. It supports advanced scanning techniques such as port scanning, service detection, OS detection, and firewall analysis. Example usage: `nmap 192.168.1.1` scans a target device to identify active ports and services.


## Whatweb

## output

<img width="812" height="524" alt="image" src="https://github.com/user-attachments/assets/6b28fbe6-c466-4ca9-99b4-330f6878970b" />

### Explanation 
The `whatweb` command is a Linux web technology identification tool used to detect technologies running on a website. It analyzes web pages and identifies details such as the web server, CMS (Content Management System), programming frameworks, analytics tools, JavaScript libraries, and security technologies being used. Cybersecurity professionals, penetration testers, and web administrators commonly use `whatweb` for reconnaissance and security assessments. The tool helps gather information about a target website before performing further testing or troubleshooting. It supports stealthy scans and detailed fingerprinting of web applications. Example usage: `whatweb example.com` displays the technologies and software associated with the target website.




## httprint
httprint -h 172.17.52.201 -s /usr/share/httprint/signatures.txt -P0 |more

## output

<img width="835" height="667" alt="image" src="https://github.com/user-attachments/assets/9b7e85f5-df26-477c-bb19-b076e1e49c04" />

### Explanation 
The `httprint` command is a web server fingerprinting tool used in Linux and cybersecurity environments to identify the type and version of web servers running on a target system. It works by sending specially crafted HTTP requests and analyzing server responses to match them against known server signatures. `httprint` is commonly used by penetration testers, ethical hackers, and network security professionals during reconnaissance and vulnerability assessment. It helps detect web servers even when server banner information is hidden or modified for security purposes. The tool supports fingerprinting of servers such as Apache, Nginx, IIS, and others. Example usage: `httprint -h example.com`.


# Tracing the Location
TCP Traceroute:
sudo traceroute -T www.google.com

## output
<img width="613" height="72" alt="Screenshot_2026-04-30_04-55-56" src="https://github.com/user-attachments/assets/31cd8c6d-1cf1-4928-86c6-6ad404bc4e0a" />

### Explanation
The TCP traceroute command is a variation of the traditional `traceroute` tool that uses TCP packets instead of ICMP or UDP packets to trace the network path between a source and destination. It is useful when firewalls or routers block standard traceroute traffic, as TCP packets are often allowed through common service ports such as port 80 (HTTP) or 443 (HTTPS). This command helps network administrators and cybersecurity professionals diagnose routing issues, analyze network paths, and test connectivity to specific services. TCP traceroute is commonly used in secure or restricted networks where normal traceroute methods fail. Example usage: `traceroute -T google.com`.


## UDP Traceroute:
sudo traceroute -U www.google.com
## output

<img width="640" height="82" alt="Screenshot_2026-04-30_04-54-40" src="https://github.com/user-attachments/assets/a4990336-8f34-4c1f-847f-a321694a8af9" />

### Explanation 
The UDP traceroute command is a network diagnostic method that uses UDP (User Datagram Protocol) packets to trace the path taken by data packets from a source system to a destination host. In Linux, the default `traceroute` command commonly sends UDP packets to high-numbered ports and monitors the responses from intermediate routers. It helps identify each network hop, measure response times, and detect routing delays or connection problems. Network administrators use UDP traceroute for troubleshooting connectivity issues and analyzing packet routes across networks. It is especially useful for understanding how data travels through routers and internet gateways. Example usage: `traceroute -U example.com`.


## ICMP Traceroute:
sudo traceroute  www.google.com
## output
<img width="676" height="82" alt="Screenshot_2026-04-30_04-53-57" src="https://github.com/user-attachments/assets/7aaa8d0d-81d9-4076-8dc8-fffdb68a7778" />

### Explanation 
The ICMP traceroute command is a network diagnostic technique that uses ICMP (Internet Control Message Protocol) echo request packets to trace the route between a source device and a destination system. Unlike the default UDP-based traceroute, this method works similarly to the `ping` command by sending ICMP packets with increasing TTL (Time To Live) values to identify each router or network hop along the path. It is commonly used by network administrators and cybersecurity professionals to troubleshoot connectivity issues, detect routing problems, and measure network latency. ICMP traceroute is especially useful when UDP traffic is restricted. Example usage: `traceroute -I google.com`.


## RESULT:
The information gathering techniques tools/procedure were  identified successfully
