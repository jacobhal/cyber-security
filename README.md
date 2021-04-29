# Cyber Security
A repository for cyber security documentation and tools.

## OWASP Dependency Checker

Detect vulnerabilities in npm packages/NuGet packages/3rd party Java libraries with this OWASP tool. Dependency checking or Software Composition Analysis (SCA), is a method of checking publicly disclosed vulnerabilities contained within our project's dependencies.

Download the command line tool and run the following command to perform an analysis:

```powershell
.\dependency-check.bat --project <project-name> --scan <folder-to-scan> --format ALL 
--out <target-folder-for-vulnerability-reports> --proxyserver <proxy-network-address> --proxyport <proxy-port>
```

> OWASP top ten Web application vulnerabilities: https://owasp.org/www-project-top-ten/

> OWASP tool download link: https://owasp.org/www-project-dependency-check/

## OWASP ZAP

Intercept requests and perform Man in the Middle attacks.

## OWASP Cheat Sheet

https://cheatsheetseries.owasp.org/

## Darknet Diares (Podcast about real world security attacks)

www.darketdiaries.com

## Microsoft Best Practices for Azure

https://docs.microsoft.com/en-us/azure/security/develop/secure-dev-overview

## Cyber Kill Chain

We need to stop/kill hackers somewhere in this chain in order to stop an attack, otherwise it's game over.

1. Reconnaissance: 
  * Find easy targets by looking at www.securityheaders.com or something similar.
  * Gather information. 
  * Check whether the sites show Server version headers in order to find versions that are vulnerable.
2. Weaponization:
  * Intruder creates remote access malware weapon, such as a virus or worm, tailored to one or more vulnerabilities.
3. Delivery:
  * Intruder transmits weapon to target (e.g., via e-mail attachments, websites or USB drives)
4. Exploitation:
  * Malware weapon's program code triggers, which takes action on target network to exploit vulnerability.
5. Installation:
  * Malware weapon installs access point (e.g., "backdoor") usable by intruder.
6. Command and Control:
  * Malware enables intruder to have "hands on the keyboard" persistent access to target network.
7. Actions on Objective:
  * Intruder takes action to achieve their goals, such as data exfiltration, data destruction, or encryption for ransom.

## Principles

### Least Privilege

Least privilege is the concept and practice of restricting access rights for users, accounts, and computing processes to only those resources absolutely required to perform routine, legitimate activities. Privilege itself refers to the authorization to bypass certain security restraints.

### Defense in Depth

The idea behind the defense in depth approach is to defend a system against any particular attack using several independent methods. It is a layering tactic, conceived by the National Security Agency (NSA) as a comprehensive approach to information and electronic security.

#### Real world example

A while back you could pass JavaScript script tags like `<script>alert('xss')</script>` in your Swish messages which would then pop up a message if you accessed your Swish transactions in your online bank.

#### Man in the Middle

Intercept requests before they reach their destination and change some data.
