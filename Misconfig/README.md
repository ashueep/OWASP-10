# Security Misconfigurations
Security Misconfigurations are distinct from the other Top 10 vulnerabilities, because they occur when security could have been configured properly but was not.

Security misconfigurations include:

1. Poorly configured permissions on cloud services, like S3 buckets
  2.  Having unnecessary features enabled, like services, pages, accounts or privileges
   3. Default accounts with unchanged passwords
   4. Error messages that are overly detailed and allow an attacker to find out more about the system
   5. Not using HTTP security headers, or revealing too much detail in the Server: HTTP header

This vulnerability can often lead to more vulnerabilities, such as default credentials giving you access to sensitive data, XXE or command injection on admin pages.

[OWASP top 10 entry for Security Misconfiguration](https://owasp.org/www-project-top-ten/2017/A6_2017-Security_Misconfiguration.html).

## Default Passwords

In October 2016, Dyn (a DNS provider) was taken offline by one of the most memorable DDoS attacks of the past 10 years. The flood of traffic came mostly from Internet of Things and networking devices like routers and modems, infected by the Mirai malware.

How did the malware take over the systems? Default passwords. The malware had a list of 63 username/password pairs, and attempted to log in to exposed telnet services.

The DDoS attack was notable because it took many large websites and services offline. Amazon, Twitter, Netflix, GitHub, Xbox Live, PlayStation Network, and many more services went offline for several hours in 3 waves of DDoS attacks on Dyn.

