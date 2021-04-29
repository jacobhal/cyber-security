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
> 

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
