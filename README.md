# Project 8 - Pentesting Live Targets

Time spent: **2** hours spent in total

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

Vulnerability #1: Session Hijacking

Vulnerability #2: SQL Injection


## Green

Vulnerability #1: Cross-Site Scripting

Vulnerability #2: User Enumeration


## Red

Vulnerability #1: Insecure Direct Object Reference

Vulnerability #2: Cross-Site Request Forgery
Red site does not validate csrf tokens allowing it to be attacked using an auto-submitting form. An attacker could use social engineering in the form of an email or using the contact form on the red website. In my gif, I have the admin copy and paste a link into the address bar. This was much easier to show off than creating a link in the contact form.

  <img src="https://github.com/jesse-ables/CodepathWeek8/blob/master/forgery.gif" width="800">


## Notes

Describe any challenges encountered while doing the work
