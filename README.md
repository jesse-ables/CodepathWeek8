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
Green site does not properly check for <script> tags in its comments page. A user can simply create a xss using <script>alert("hacking happening now")</script>
  
  <img src="https://github.com/jesse-ables/CodepathWeek8/blob/master/xss.gif" width="800">

Vulnerability #2: User Enumeration


## Red

Vulnerability #1: Insecure Direct Object Reference
Red site has certain staff member data that is not supposed to be seen by the public. It can be accessed by using the url: https://<span></span>xx.xxx.xx.xxx/red/public/salesperson.php?id=[enter number here]. A user can simply change the number at the end to access hidden data.

  <img src="https://github.com/jesse-ables/CodepathWeek8/blob/master/IDOR.gif" width="800">

Vulnerability #2: Cross-Site Request Forgery
Red site does not validate csrf tokens allowing it to be attacked using an auto-submitting form. An attacker could use social engineering in the form of an email or using the contact form on the red website. In my gif, I have the admin copy and paste a link into the address bar. This was much easier to show off than creating a link in the contact form.

  <img src="https://github.com/jesse-ables/CodepathWeek8/blob/master/forgery.gif" width="800">


## Notes

The most complicated part was finding certain attack surfaces. I didn't realize that the SQLi attack would be done inside of a url.

On a small note, it is possible to create a small availability attack on a certain part of the green site by creating an auto submitting form in the contact us page. It will always attempt to submit, making it impossible to view comments from customer. Maybe this is considered a DOS attack. 
