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
  