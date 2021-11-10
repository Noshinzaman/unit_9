# unit_9# Project 9 - Pentesting Live Targets

Time spent: **2** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:

* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each color is vulnerable to only 2 of the 6 possible exploits. First discover which color has the specific vulnerability, then write a short description of how to exploit it, and finally demonstrate it using screenshots compiled into a GIF.

## Blue

Vulnerability #1: ____SQL Injection______________

Description: After the link inject SQL(' OR SLEEP(5)=0--')

<img src="https://user-images.githubusercontent.com/89932088/141192650-9a971cfa-62c2-45a2-b12a-7797d4bedee3.gif">

Vulnerability #2: __Session Hijacking________________

Description: When the admin is logged in, attacker is able to steal the session of admin and can bupass logging in with username and password.

<img src="https://user-images.githubusercontent.com/89932088/141192785-a56d52c4-2a6b-4bb8-bc2e-f9ba76e7c1af.gif">

## Green

Vulnerability #1: __XSS________________

Description: found XSS exploit.i am able to reflected XSS attack.

<img src="https://user-images.githubusercontent.com/89932088/141192943-a66513d2-b3c1-47e2-afc3-d0e2656256c0.gif">

Vulnerability #2: ___________User Enumeration_______

Description:
1)login and type a username ypu know exists in the database and type a wrong password.
2)A username that exists on the database with a wrong password will be printed in bold.
3) But a username that does not exist with inputted wrong password will not be in bold.


<img src="https://user-images.githubusercontent.com/89932088/141194102-3898c17f-29a1-4d85-8eef-ab5d5761148c.gif">


## Red

Vulnerability #1: __________IDOR________

Description:1) when you check the list of salesperson on the site, there is an extension of an id parameter which is fixed and exploitable.
2)Change the id parameter until you get a hidden/unknown/secret employee/salesperson.

<img src="https://user-images.githubusercontent.com/89932088/141192263-db24ae16-cba1-4435-ad1c-cc867d1dd921.gif">

Vulnerability #2: _____CSRF_____________

Description:
1) There is a vulnerability in the users section of Globitek Red
2) Go to users page and inspect page source
3) Create a new html file that takes form and resubmits it without using the csrf token.
4) Open the vulnerable html file and watch it change user information directly on the website.

<img src="https://user-images.githubusercontent.com/89932088/141193295-73ad120b-f8c3-45bd-bb9b-72b023ae167c.gif">

Bonus Objectives

Vulnerability #1: __XSS_attack_______________

Description: write a feedback so that when admin presses and checks on it, while be vulnerable to XSS attack that direct the user to a new URL.

<img src="https://user-images.githubusercontent.com/89932088/141193371-643ee963-a6c3-4bcd-b926-f7b31ee87e20.gif">


## Notes

Describe any challenges encountered while doing the work



