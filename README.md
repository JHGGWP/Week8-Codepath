# Week8-Codepath

# Project 8 - Pentesting Live Targets

Time spent: **10** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1: _____SQL Injection___

GIF Walkthrough: 


* The exploit is in the URL https://35.184.88.145/blue/public/staff/salespeople/show.php?id=????
* put 'OR SLEEP(5)=0--' to replace ??. The 5 means sleeping for 5 seconds.

Vulnerability #2: _____Session Hijacking_______

GIF Walkthrough: 

* First log in on Chrome and get the session ID at public/hacktools/change_session_id.php page
* Change the sessionID at public/hacktools/change_session_id.php from a different browser
* You can successfully log in to the account you never put the password in


## Green

Vulnerability #1: _____XSS_________

GIF Walkthrough: 

* This exploit is done via the feedback section.
* You can view the injection in the "Feedback" section

Vulnerability #2: _____User Enumeration____

GIF Walkthrough: 

* Using the given username "pperson" we can see that a valid username shows a bold error.
* An incorrect username shows a not-bolded error.

## Red

Vulnerability #1: ______IDOR______

GIF Walkthrough:

* Do not log in
* Change the id to find the user which is not published yet

Vulnerability #2: ______CSRF______

GIF Walkthrough:

## Notes

Describe any challenges encountered while doing the work
