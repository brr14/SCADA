# Metasploit
Started with running the basic commands like:</br>

* *help* displays all of the commands and it's functions.</br>
* *use* loads the required module.</br>
* *show options* displays all the options that need to be set before running the module like IP addresses,ports,etc.</br>
* *show targets* displays the list of targets the exploit will work against.</br>
* *info* displays key information about the selected module.</br>


**Variables used in exploits:**

* *RHOSTS* this is the remote hosts or target IPs.
* *LHOST* this for local host or attacker IP.
* *RPORT* this is the remote port or target port.
* *LPORT* this is the local port or attacker port.

**Metasploit Modules**

![Screenshot from 2023-03-10 22-42-34](https://user-images.githubusercontent.com/96241263/224387702-de272907-8dad-46a9-8f1f-fd3b8b36dbfd.png)
* *Exploits* they define the exploitation framework which take advantage of a vulnerability in a system.
* *Payloads* these help in connecting the target system.
* *Auxiliary* provides capabilities like scanners,DoS,spoofing,etc.
* *Encoders* designed to re-encode payloads and exploits.
* *Post* (post exploitation) used after exploitation of the system.
* *NOPS* (no operation) which causes the sytem to not do anything for a clock cycle.
