# Cyber Security
A repository for cyber security documentation and tools.

## OWASP Dependency Checker

Detect vulnerabilities in npm packages/NuGet packages/3rd party Java libraries with this OWASP tool. Dependency checking or Software Composition Analysis (SCA), is a method of checking publicly disclosed vulnerabilities contained within our project's dependencies.

Download the command line tool and run the following command to perform an analysis:

```powershell
.\dependency-check.bat --project <project-name> --scan <folder-to-scan> --format ALL --out <target-folder-for-vulnerability-reports> --proxyserver <proxy-network-address> --proxyport <proxy-port>
```

> OWASP top ten Web application vulnerabilities: https://owasp.org/www-project-top-ten/

> OWASP tool download link: https://owasp.org/www-project-dependency-check/
