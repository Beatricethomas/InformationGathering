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


## Finding IP address:
ping command is available on Windows as well as on Linux OS. Following is the example to find out the IP address of facebook.com.
##output
<img width="649" height="238" alt="Screenshot_2026-04-30_04-34-28" src="https://github.com/user-attachments/assets/76974f7f-8536-4c29-ad21-fcf423571716" />



## Finding Hosting Company
get further detail by using ip2location.com website.

## output

<img width="1754" height="851" alt="Screenshot_2026-04-30_04-37-59" src="https://github.com/user-attachments/assets/e11bd466-23cf-40b2-849d-7d9f0b5032b3" />

<img width="1754" height="851" alt="Screenshot_2026-04-30_04-37-59" src="https://github.com/user-attachments/assets/03fa17b8-e6cc-4c68-92ac-2dc596a2bede" />

## History of the website:
## output
https://web.archive.org/

<img width="1736" height="824" alt="Screenshot_2026-04-30_04-44-07" src="https://github.com/user-attachments/assets/fd4a0c7d-fae8-482f-87ba-d30eb50c6a79" />
<img width="1303" height="767" alt="Screenshot_2026-04-30_04-44-27" src="https://github.com/user-attachments/assets/4684afbb-9f26-4b1b-9089-ce6b9f4c529b" />


# Webserver Fingerprinting:

## Netcat:
sudo nc example.com 80
GET / HTTP/1.1
Host: example.com
<img width="226" height="96" alt="Screenshot_2026-04-30_04-51-58" src="https://github.com/user-attachments/assets/9fc5e4db-06f3-4c4b-b8c0-17ab93827d15" />



## nmap:
## output
<img width="913" height="240" alt="Screenshot_2026-04-30_04-49-39" src="https://github.com/user-attachments/assets/01382d56-51b0-453f-a787-63a1fd166350" />


## Whatweb
## output


## httprint
## output




# Tracing the Location
TCP Traceroute:
sudo traceroute -T www.google.com
## output
<img width="613" height="72" alt="Screenshot_2026-04-30_04-55-56" src="https://github.com/user-attachments/assets/31cd8c6d-1cf1-4928-86c6-6ad404bc4e0a" />


## UDP Traceroute:
sudo traceroute -U www.google.com
## output

<img width="640" height="82" alt="Screenshot_2026-04-30_04-54-40" src="https://github.com/user-attachments/assets/a4990336-8f34-4c1f-847f-a321694a8af9" />


## ICMP Traceroute:
sudo traceroute  www.google.com
## output
<img width="676" height="82" alt="Screenshot_2026-04-30_04-53-57" src="https://github.com/user-attachments/assets/7aaa8d0d-81d9-4076-8dc8-fffdb68a7778" />

## RESULT:
The information gathering techniques tools/procedure were  identified successfully
