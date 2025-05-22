## Offensive Security 
The core of of offensive security involves breaking into computer systems, exploiting software bugs and finding loopholes in the applications to gain unauthorized access. 

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