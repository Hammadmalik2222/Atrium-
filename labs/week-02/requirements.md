# Week 2 security requirements

Your name: Hammad Malik 
Student ID: 20073974
Date: 1/10/2026

---

## 1. What this application is

Atrium is a workspace that helps to manage everyday tasks that a motive to kept people,
resources & practical knwoledge together. You can sign in with 3 different credentials either it is member or admin. After sign in, we have a dashboard with the information of staff, different forms & profile information. 


## 2. What is worth protecting

Four assets.

| Asset |What it costs if this goes wrong|

| Application |if the server/application is down so users will not do any type of work on it|

| Admin Account |As we know, Admin account is the most powerful asset of any organization because it has all rights rather than other users. if this account has been accessed by outsider that means whole system will be in danger|

| Staff Login Credentials |if any outsiders access any staff login information, they can simply login & access the company plan/registers/guides. They might be change any important data on registers or they might be just kept silent to know all the future plans on Atrium|

| Users Personal data (Email) |if any outsiders access staff directory & access their personal data, they can send phishy emails to all staff on daily basis if anyone just click on it may be mistakenly they can easily access Atrium & can do anything with platform|


## 3. The requirements

***Assistant***
- It is not allowed for any unauthorised person to access Atrium, its dashboard, staff pages, or any authenticated section of the app, because the system is meant only for valid staff and admin users.
- It is not allowed for any user to share, guess, steal, or reuse another person’s login credentials, because each account belongs to one authorised person and must be used only by that person.
***Myself***
- It is not allowed to any staff users to access & CRUD(create,read,update & delete) any file of others staff.
- Every user have a right to change their passwords under the Application Security Verifications Standard of OWASP.


## 4. One I rejected or rewrote

- The original sentence: It is not allowed for any unauthorised person to access Atrium, its dashboard, staff pages, or any authenticated section of the app, because the system is meant only for valid staff and admin users.
- My version: if any unauthorised person will request to access /dashboard or /staff or any other authenticated page route, it will be redirected to /login page.
- Which test it failed, and why: somebody could check it because on a browser somebody will may access these URL through basic route names.

## 5. How somebody would check one of these

Pick one requirement. Write the steps for a person who has never seen Atrium and
cannot ask you anything.

- The requirement: Authorised person request to /dashboard & /staff
- Sign in as: N / A 
- Steps: 
    1.Download & start Atrium by following instructions. 
    2.Open new browser & type in address bar "http://localhost:9090/dashboard" without login.
    3.Press Enter  
- What result would mean the requirement is met: will not access the dashboard page, just redirect to login page
- What result would mean it is not met: will access the dashboard page.

---

