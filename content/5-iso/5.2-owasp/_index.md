---
title : "OWASP Top 10"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 5.2 </b> "
---



#### [Learning the OWASP Top 10](https://www.linkedin.com/learning/learning-the-owasp-top-10-9364599/broken-access-control?autoSkip=true&resume=false&u=103729754)

OWASP stands for Open Web Application Security Project. For decades, this group has been providing resources to educate and inform technology professionals about security best practices. 

1. Broken access control
2. Cryptographic failures
3. Injection
4. Insecure design
5. Security misconfiguration
6. Vulnerable and outdated components
7. Identification and authentication
8. Software and data integrity failures
9. Securiy logging and monitoring failures
10. Server-side request forgery (SSRF)

https://owasp.org/www-project-top-ten/

- Key Takeaways:

![52](/secu/images/5/52/111.png?featherlight=false&width=50pc)

- Question:
  - 1: Which statement describes broken access control in a web application?
    - Private information is sent to an unauthorized person.
    - Private information is exposed to an unauthorized person.
    - Private information can be read, edited, or deleted by an unauthorized person.
  - 2: Why do vulnerable and outdated components have such a large impact on the security of web applications?
    - Most web apps include several different components, all of which must be tracked and kept up to date in order to improve the security posture of the application.
  - 3: How do you know whether each of your components is vulnerable or not?
    - Research known vulnerabilities as well as proactively test your applications.
    - You should then update any out-of-date software and patch known vulnerabilities.
  - 4: If you know that legitimate external resources are coming from a specific location, what can you do to prevent SSRF?
    - Allow only that IP address or host name.
    - You know that legitimate resources are coming from a specific location, so enforce an only-allowed list to prevent SSRF.
  - 5: What is the significance of the new Insecure Design category in the 2021 OWASP Top 10?
    - This new category acknowledges that security matters in the requirements and design phase of web app development.
  - 6: What is an example of a digital security misconfiguration?
    - You choose not to use a password on your mobile device.
    - If you are choosing not to use a password on your mobile device, then your setup is not very secure.
  - 7: Why is security logging and monitoring so important?
    - It allows breaches to be discovered more quickly and at earlier stages of an attack.
  - 8: If you are storing sensitive data, when should you encrypt the data?
    - when the data is at rest and in transit
    - Any data left unencrypted is at risk, so you should encrypt sensitive data that you are storing.
  - 9: Why don't regular access controls always work to prevent a server side request forgery (SSRF) attack?
    - The server may have privileged access.
  - 10: What is the result of an injection attack?
    - The web application interprets input submitted by the user as an instruction to follow.
  - 11: Which scenario is an example of identification and authentication failure?
    - when a web app establishes a new user session without closing out the previous one
    - when the software communicates with a host that provides a certificate, but does not ensure that the certificate is actually associated with that host
    - when an actor claims to have a given identity, and the software does not prove that the claim is correct
  - 12: The eighth item, Software and Data Integrity Failures, is a subset of what other OWASP top 10 item?
    - Vulnerable and Outdated Components
    - The eighth item is actually a subset of the sixth, specifically, vulnerabilities that result from an insecure CI/CD pipeline.

| 1. Broken access control | - |
|---|---|
|![52][1]| ![52][2]|
|![52][3]| ![52][4]|

{{%expand "Senario" %}}
|- | - |
|---|---|
|![52](/secu/images/5/52/5.png?featherlight=false&width=50pc)|![52](/secu/images/5/52/6.png?featherlight=false&width=50pc)|
|![52](/secu/images/5/52/7.png?featherlight=false&width=50pc)|![52](/secu/images/5/52/8.png?featherlight=false&width=50pc)|
|![52](/secu/images/5/52/9.png?featherlight=false&width=50pc)|![52](/secu/images/5/52/10.png?featherlight=false&width=50pc)|
|![52](/secu/images/5/52/11.png?featherlight=false&width=50pc)|![52](/secu/images/5/52/12.png?featherlight=false&width=50pc)|
|![52](/secu/images/5/52/13.png?featherlight=false&width=50pc)|![52](/secu/images/5/52/14.png?featherlight=false&width=50pc)|
|![52](/secu/images/5/52/15.png?featherlight=false&width=50pc)|![52](/secu/images/5/52/16.png?featherlight=false&width=50pc)|
{{% /expand%}}

| 2. Cryptographic Failures | - |
|---|---|
|![52][21]| ![52][22]|
|![52][23]| ![52][24]|

| 3. Injection | - |
|---|---|
|![52][31]| ![52][32]|
|![52][33]| ![52][36]|
|![52][34]| ![52][35]|

| 4. Insecure design | - |
|---|---|
|![52][41]| ![52][44]|

{{%expand "Noted of Insecure Design" %}}
|- | - |
|---|---|
|![52](/secu/images/5/52/42.png?featherlight=false&width=50pc)|![52](/secu/images/5/52/43.png?featherlight=false&width=50pc)|
{{% /expand%}}

| 5. Security misconfiguration | - |
|---|---|
|![52][51]| ![52][57]|
|![52][55]| ![52][56]|

{{%expand "Noted " %}}
|- | - |
|---|---|
|![52](/secu/images/5/52/52.png?featherlight=false&width=50pc)||
|![52](/secu/images/5/52/53.png?featherlight=false&width=50pc)|![52](/secu/images/5/52/54.png?featherlight=false&width=50pc)|
{{% /expand%}}

| 6. Vulnerable and outdated components | - |
|---|---|
|![52][61]| ![52][62]|
|![52][64]| ![52][65]|
{{%expand "Noted of Insecure Design" %}}
|- | - |
|---|---|
|![52](/secu/images/5/52/63.png?featherlight=false&width=50pc)||
{{% /expand%}}

| 7. Identification and authentication| - |
|---|---|
|![52][71]| ![52][72]|
|![52][75]| |

{{%expand "Noted" %}}
|- | - |
|---|---|
|![52](/secu/images/5/52/73.png?featherlight=false&width=50pc)|![52](/secu/images/5/52/74.png?featherlight=false&width=50pc)|
|![52](/secu/images/5/52/76.png?featherlight=false&width=50pc)|![52](/secu/images/5/52/77.png?featherlight=false&width=50pc)|
{{% /expand%}}

| 8. Software and data integrity failures | - |
|---|---|
|![52][81]| ![52][82]|
|![52][85]| ![52][86]|

{{%expand "Noted" %}}
|- | - |
|---|---|
|![52](/secu/images/5/52/83.png?featherlight=false&width=50pc)|![52](/secu/images/5/52/84.png?featherlight=false&width=50pc)|
{{% /expand%}}

| 9. Security logging and monitoring failures | - |
|---|---|
|![52][91]| ![52][92]|
|| ![52][97]|

{{%expand "Noted " %}}
|- | - |
|---|---|
|![52](/secu/images/5/52/93.png?featherlight=false&width=50pc)|![52](/secu/images/5/52/94.png?featherlight=false&width=50pc)|
|![52](/secu/images/5/52/95.png?featherlight=false&width=50pc)|![52](/secu/images/5/52/96.png?featherlight=false&width=50pc)|
{{% /expand%}}

| 10. Server-side reuest forgegy (SSRF)| - |
|---|---|
|![52][101]| ![52][102]|
|| ![52][105]|
{{%expand "Noted" %}}
|- | - |
|---|---|
|![52](/secu/images/5/52/103.png?featherlight=false&width=50pc)|![52](/secu/images/5/52/104.png?featherlight=false&width=50pc)|
{{% /expand%}}

[1]: /secu/images/5/52/1.png?featherlight=false&width=40pc
[2]: /secu/images/5/52/2.png?featherlight=false&width=40pc
[3]: /secu/images/5/52/3.png?featherlight=false&width=40pc
[4]: /secu/images/5/52/4.png?featherlight=false&width=40pc
[5]: /secu/images/5/52/5.png?featherlight=false&width=40pc
[6]: /secu/images/5/52/6.png?featherlight=false&width=40pc
[7]: /secu/images/5/52/7.png?featherlight=false&width=40pc
[8]: /secu/images/5/52/8.png?featherlight=false&width=40pc
[9]: /secu/images/5/52/9.png?featherlight=false&width=40pc
[10]: /secu/images/5/52/10.png?featherlight=false&width=40pc
[11]: /secu/images/5/52/11.png?featherlight=false&width=40pc
[12]: /secu/images/5/52/12.png?featherlight=false&width=40pc
[13]: /secu/images/5/52/13.png?featherlight=false&width=40pc
[14]: /secu/images/5/52/14.png?featherlight=false&width=40pc
[15]: /secu/images/5/52/15.png?featherlight=false&width=40pc
[16]: /secu/images/5/52/16.png?featherlight=false&width=40pc

[21]: /secu/images/5/52/21.png?featherlight=false&width=40pc
[22]: /secu/images/5/52/22.png?featherlight=false&width=40pc
[23]: /secu/images/5/52/23.png?featherlight=false&width=40pc
[24]: /secu/images/5/52/24.png?featherlight=false&width=40pc
[25]: /secu/images/5/52/25.png?featherlight=false&width=40pc
[26]: /secu/images/5/52/26.png?featherlight=false&width=40pc
[27]: /secu/images/5/52/27.png?featherlight=false&width=40pc

[31]: /secu/images/5/52/31.png?featherlight=false&width=40pc
[32]: /secu/images/5/52/32.png?featherlight=false&width=40pc
[33]: /secu/images/5/52/33.png?featherlight=false&width=40pc
[34]: /secu/images/5/52/34.png?featherlight=false&width=40pc
[35]: /secu/images/5/52/35.png?featherlight=false&width=40pc
[36]: /secu/images/5/52/36.png?featherlight=false&width=40pc

[41]: /secu/images/5/52/41.png?featherlight=false&width=40pc
[42]: /secu/images/5/52/42.png?featherlight=false&width=40pc
[43]: /secu/images/5/52/43.png?featherlight=false&width=40pc
[44]: /secu/images/5/52/44.png?featherlight=false&width=40pc
[45]: /secu/images/5/52/45.png?featherlight=false&width=40pc

[51]: /secu/images/5/52/51.png?featherlight=false&width=40pc
[52]: /secu/images/5/52/52.png?featherlight=false&width=40pc
[53]: /secu/images/5/52/53.png?featherlight=false&width=40pc
[54]: /secu/images/5/52/54.png?featherlight=false&width=40pc
[55]: /secu/images/5/52/55.png?featherlight=false&width=40pc
[56]: /secu/images/5/52/56.png?featherlight=false&width=40pc
[57]: /secu/images/5/52/57.png?featherlight=false&width=40pc

[61]: /secu/images/5/52/61.png?featherlight=false&width=40pc
[62]: /secu/images/5/52/62.png?featherlight=false&width=40pc
[63]: /secu/images/5/52/63.png?featherlight=false&width=40pc
[64]: /secu/images/5/52/64.png?featherlight=false&width=40pc
[65]: /secu/images/5/52/65.png?featherlight=false&width=40pc
[66]: /secu/images/5/52/66.png?featherlight=false&width=40pc

[71]: /secu/images/5/52/71.png?featherlight=false&width=40pc
[72]: /secu/images/5/52/72.png?featherlight=false&width=40pc
[73]: /secu/images/5/52/73.png?featherlight=false&width=40pc
[74]: /secu/images/5/52/74.png?featherlight=false&width=40pc
[75]: /secu/images/5/52/75.png?featherlight=false&width=40pc
[76]: /secu/images/5/52/76.png?featherlight=false&width=40pc

[81]: /secu/images/5/52/81.png?featherlight=false&width=40pc
[82]: /secu/images/5/52/82.png?featherlight=false&width=40pc
[83]: /secu/images/5/52/83.png?featherlight=false&width=40pc
[84]: /secu/images/5/52/84.png?featherlight=false&width=40pc
[85]: /secu/images/5/52/85.png?featherlight=false&width=40pc
[86]: /secu/images/5/52/86.png?featherlight=false&width=40pc

[91]: /secu/images/5/52/91.png?featherlight=false&width=40pc
[92]: /secu/images/5/52/92.png?featherlight=false&width=40pc
[93]: /secu/images/5/52/93.png?featherlight=false&width=40pc
[94]: /secu/images/5/52/94.png?featherlight=false&width=40pc
[95]: /secu/images/5/52/95.png?featherlight=false&width=40pc
[96]: /secu/images/5/52/96.png?featherlight=false&width=40pc
[97]: /secu/images/5/52/97.png?featherlight=false&width=40pc

[101]: /secu/images/5/52/101.png?featherlight=false&width=40pc
[102]: /secu/images/5/52/102.png?featherlight=false&width=40pc
[103]: /secu/images/5/52/103.png?featherlight=false&width=40pc
[104]: /secu/images/5/52/104.png?featherlight=false&width=40pc
[105]: /secu/images/5/52/105.png?featherlight=false&width=40pc
[106]: /secu/images/5/52/106.png?featherlight=false&width=40pc