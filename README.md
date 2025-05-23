## Offensive Security 
The core of of offensive security involves breaking into computer systems, exploiting software bugs and finding loopholes in the applications to gain unauthorized access. 
**Red teams**  and **Penetration testers** specialize in offensive techniques. 

The goal is to understand hacker tatctics and enhance our system defences. 

# Task 1: hacking your first machine 

1. Using a fake bank application, the goal was to exploit valunarabilties on within their web app. 
2. Virtual machine was created to simulate an environment to practice within.
3. The command -line application was used to execute the commends need to exploit the web app. 
4. Use Gobuster to brute-force FakeBank's website. command use(gobuster -u http://fakebank.thm -w wordlist.txt dir)
  **-u: used to state the website we're scanning.**
  **-w: takes a list of words to iterate through to find hidden pages.**

5. Gobuster scans the website with each word in the list, finding pages that exit on the site. The pages in the list of page/directory names (indicated by Status: 200)
**Status: 200 indicates the  request was successful**

6. Using the bank-transfer page, we can access that page unauthorized and transfer $2000 ffrom account number 2276 to 8881. 

7. Hack was succesfull with a massage returned **BANK-HACKED**


### Gobuster- is a brute-force scanner too to enumaerate directories and files of websites. Also assist in finding DNS subdomain and virtual host names. 


# Defensive Security
**Blue teams** are part of the defensive security landscape. 
Defensive security is concerned with two main tasks:
1. Preventint intrusions from occurring 
2. Detecting intrusions when they occur and responding properly. 

Some of the tasks that are related to defensive security include:

    User cyber security awareness: Training users about cyber security helps protect against attacks targeting their systems.
    Documenting and managing assets: We need to know the systems and devices we must manage and protect adequately.
    Updating and patching systems: Ensuring that computers, servers, and network devices are correctly updated and patched against any known vulnerability (weakness).
    Setting up preventative security devices: firewall and intrusion prevention systems (IPS) are critical components of preventative security. Firewalls control what network traffic can go inside and what can leave the system or network. IPS blocks any network traffic that matches present rules and attack signatures.
    Setting up logging and monitoring devices: Proper network logging and monitoring are essential for detecting malicious activities and intrusions. If a new unauthorized device appears on our network, we should be able to detect it.


### Areas of Defensive Security
#### Summmary

Security Operations Center (SOC)
 A Security Operation Center(SOC) is a team of cyber security professionals that monitors the network and its systems to detect malicious cyber secuirity events. 
  SOC is interested in:
  1. Vulnerabilites 
  2. Policy voilations 
  3. Unauthorized activity 
  4. Network intrusion. 


  **Threat Intelligence**
  Key terms:
  - Intelligence: information gathered about actual and potential enemies. 
  - Threat: any action that can disrupt or adversely affect the system. 

  Threat Intelligence collects information to help the company better prepare against potential adversaries. 
    Intelligence needs data. Data has to be collected, processed, and analyzed. Data is collected from local sources such as network logs and public sources such as forums. Data processing arranges it into a format suitable for analysis. The analysis phase seeks to find more information about the attackers and their motives; moreover, it aims to create a list of recommendations and actionable steps.

    Learning about your adversaries lets you know their tactics, techniques, and procedures. As a result of threat intelligence, we identify the threat actor (adversary) and predict their activity. Consequently, we can mitigate their attacks and prepare a response strategy.


    ### Digital Forensics and Incident Response (DFIR)
    1. Digital Forensics: 
      Forensics is the application of science to investigate crimes and establish facts. With the use and spread of digital systems, such as computers and smartphones, a new branch of forensics was born to investigate related crimes: computer forensics, which later evolved into digital forensics.

    2. Incident Response
      An incident usually refers to a data breach or cyber attack; however, in some cases, it can be something less critical, such as a misconfiguration, an intrusion attempt, or a policy violation. Examples of a cyber attack include an attacker making our network or systems inaccessible, defacing (changing) the public website, and data breach (stealing company data). How would you respond to a cyber attack? Incident response specifies the methodology that should be followed to handle such a case. The aim is to reduce damage and recover in the shortest time possible. Ideally, you would develop a plan that is ready for incident response.

  The four major phases of the incident response process are:

    Preparation: This requires a team trained and ready to handle incidents. Ideally, various measures are put in place to prevent incidents from happening in the first place.
    Detection and Analysis: The team has the necessary resources to detect any incident; moreover, it is essential to analyze any detected incident further to learn about its severity.
    Containment, Eradication, and Recovery: Once an incident is detected, it is crucial to stop it from affecting other systems, eliminate it, and recover the affected systems. For instance, when we notice that a system is infected with a computer virus, we would like to stop (contain) the virus from spreading to other systems, clean (eradicate) the virus, and ensure proper system recovery.
    Post-Incident Activity: After a successful recovery, a report is produced, and the lesson learned is shared to prevent similar future incidents.


    3. Malware Analysis
    Malware stands for malicious software. Software refers to programs, documents, and files you can save on a disk or send over the network. Malware includes many types, such as:

    A virus is a piece of code (part of a program) that attaches itself to a program. It is designed to spread from one computer to another and works by altering, overwriting, and deleting files once it infects a computer. The result ranges from the computer becoming slow to unusable.
    Trojan Horse is a program that shows one desirable function but hides a malicious function underneath. For example, a victim might download a video player from a shady website that gives the attacker complete control over their system.
    Ransomware is a malicious program that encrypts the user’s files. Encryption makes the files unreadable without knowing the encryption password. The attacker offers the user the encryption password if the user is willing to pay a “ransom.”


  ## Task 2: Practical example of defensive secuirity 

  SIEM (Security Information and Event Management) tool - gathers security-related information and events from various sources and present them in one dashboard. . If the SIEM finds something suspicious, an alert will be generated.

  - Flag: is a series of characters with format like THM{RANDOM_WORDS}

  At the end of the task, the asnwer was THM{THREAT-BLOCKED}. 


## Networking 

Network- a computer network is a group of interconnected nodes or computing devices that exchange data and reseources with each other. 

Devices that are connected together.

#### Internet 
The internet is a global network of linked computers, servers, phones and smart appliances that communicate with each other using the transmission control protocol (TCP) standard to enable the fast exchange of information and files, along  with other types of services. 
*Tim Berners-Lee*

  Network can be one of two types:
  1. A privite network
  2. A public network 

### Identifying Devices on a Network
To communicate and maintain order, devices must be both Identifying and identifiable on a network. 
Devices on a network are very similar to humans in the fact that we have two ways of being identified:
  1. Our Name
  2. Our Fingerprints

Devices have the same two means of identification with one vbeing permeable. :
  1. An IP Address 
  2. A Media Access Control (MAC) Address


  #### IP Addresses 
  An IP address or Internet Protocol address can be used as a way of identifying a host on a network for a period of time, where taht IP address can then be associated with another device without the IP address changing. 

  IP adddress is a set of numbers that are divied into f0ur octets. 
  Octets repesents a value between 0 and 255. A unit of digital information. 

An IP address is a set of numbers that are divided into four octets. The value of each octet will summarise to be the IP address of the device on the network. This number is calculated through a technique known as IP addressing & subnetting, but that is for another day. What's important to understand here is that IP addresses can change from device to device but cannot be active simultaneously more than once within the same network.

IP Addresses follow a set of standards known as protocols. These protocols are the backbone of networking and force many devices to communicate in the same language, which is something that we'll come onto another time. However, we should recall that devices can be on both a private and public network. Depending on where they are will determine what type of IP address they have: a public or private IP address.

A public address is used to identify the device on the Internet, whereas a private address is used to identify a device amongst other devices. Take the table & screenshot below as an example. Here we have two devices on a private network:

Device Name	IP Address	IP Address Type
DESKTOP-KJE57FD	192.168.1.77	Private
DESKTOP-KJE57FD	86.157.52.21	Public
CMNatic-PC	192.168.1.74	Private
CMNatic-PC	86.157.52.21
	Public


  ### MAC Addresses 
  The devices on the internet will have a phisical network interface, which is a microchip board found on the device's motherboard. 
  
  The network interface is assigned a unique address at the factory  it was built at, called  a **MAC(Media Access Control) address. The MAC address is a **twelve-charecter** hexidecimal** number(a base sixteen numbering system used in computing to represent numbers) split into two's and separeated by colon.These colons are considered separators. For example, a4:c3:f0:85:ac:2d. The first six characters represent the company that made the network interface, and the last six is a unique number.


  **Mac addresses can be "spoofed".**
  Spoofing occurs when a network device pretends to dentify as another using its MAC address. When this occurs, it can often break poorly implemented security designs that assumes that devices talking on a network are trustworthy. 

  ## PRACTICAL  
Spoofing: 
Goal- To pretend to identify as another networdked device using device's MAC address. 

Did this by changing my MAC address to a another device's MAC address to get on a hotal Wi-Fi that i was supposed to pay for. 

THM{YOU_GOT_ON_TRYHACKME}