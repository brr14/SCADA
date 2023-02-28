# Vulnerabilities in SCADA systems
Since SCADA systems oversees a large number of devices it gives a wider attack surface 
Some vulnerabilities that exist are the ones that were easily detectable by shodan, it was easy to access web cameras that were positioned in different countries, I was able to refine the data by place, port number,etc.

**Where can they be found?**
* *HMI* - Human-machine interface are used to display data from various parts of the SCADA system to help make decisions based on the data transmitted. These machines can be an ideal target for hackers to gain access over these running processes.

* *Apps and Web Interfaces* - These help in connecting the engineers with PLCs and RTUs over internet and monitor them remotely. Since these are connected over internet they are more prone to attackers influencing the industrial processes.

* *Protocols* - SCADA uses multiple protocols such as Modbus, Profinet,etc. to control and monitor different processes but they lack security capabilities which could lead to malfunction of the system if the attacker alters the data that is being sent through the modbus protocol to the PLCs and RTUs.

**Some notable attacks on SCADA systems**
* *Stuxnet worm(2010)*- This worm destroyed numerous centrifuges in Iran's uranium enrichment facility by causing them to burn themselves out. It travelled on USB sticks and spread through Microsoft Windows computers where it targeted PLCs and sent malicious information through them to the system while sending false feedback to the main controller.

* *Flame(2012)*- It is believed to have been developed by a nation state for cyber espionage purpose which was used to target Windows os by capturing screenshots, recording keystrokes and eavesdropping on conversations through computer's mic. It has the ability to spread through a network which infects the other systems connected through the same network. This malware targeted organisations in the Middle East.

* *Havex(2013)*- Similar to flame this was also used for cyber espionage purpose where it sent out spear-phising emails that contain malicious links which once installed, it is able to collect information like device names, model numbers and firmware versions about the ICS systems connected to that computer.

* *Industroyer(2016)*- It is a type of malware designed to target ICS used in critical infrastructure, such as power grids, water treatment plants,etc. It was used in a cyberattack on the ukranian power grid that caused a widespread blackout. This is considered to be the most sophisticated malware developed to target ICS.

* *Triton(2017)*- Triton is notable for its ability to directly target the safety systems of ICS, which are designed to prevent accidents and protect workers from harm. Specifically, Triton is designed to target the Triconex Safety Instrumented System (SIS), a type of safety system used in many industrial facilities.


