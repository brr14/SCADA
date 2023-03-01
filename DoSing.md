# DoSing a SCADA site 

**What is DoS attack?**
* It is a Denial of Service attack which shuts down the machine or network making it inaccessible for the user or simply exploit vulnerabilities that cause the target system to crash.These kind of attacks can lead to electrical breakouts, shutdown of water plants,etc.</br>
* There are 2 methods of DoS attacks: flooding services or crashing services.

*Flood attacks* occur when the system receives too much traffic for the server to buffer causing them to slow down.</br>

Examples- *Buffer overflow attack* (hacker sends in more traffic to the network address that what it is capable of handling)</br>

*ICMP flood* (leverages misconfigured network devices by sending spoofed packets that ping every computer on the targeted network, instead of just one specific machine. The network is then triggered to amplify the traffic. This attack is also known as the smurf attack or ping of death)</br>

*SYN flood* (sends a request to connect to a server, but never completes the handshake. Continues until all open ports are saturated with requests and none are available for legitimate users to connect to)</br>

* Used sample pcap file to analyse modbus diagnostic functions in wireshark.



