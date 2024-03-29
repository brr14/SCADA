# Introduction
SCADA systems are used to protect the process while IT systems are used to protect the data.

## Why do we need to protect the process?
Scada systems are used to monitor the processes that are being executed with no issues . It is dependent on continuous processing so a single valve malfunction can cause problem in the entire plant.For example the texas city oil refinery blew up in 2005 beacause a pressure releif valve malfunctioned.

### Protocols in scada systems
(a) **MODBUS**- It is a serial communication protocol developed by Modicon for it's use with PLCs. It helps in transmitting information between the instrumentation and control devices send back information to the main controller. Modbus is often used to connect a supervisory computer with a remote terminal unit (RTU) in supervisory control and data acquisition (SCADA)systems.It requires little processing power since it is based on master/slave architecture which works on a request/reply model.


Basic Working- The data is transmitted in the form of a series of zeroes and ones called bits. Each bit is sent as a voltage. Zeroes are sent as positive voltages and ones are negative, typical transmission speed is 9600 baud (bits/sec). 

* *Modbus(RTU)*- Modbus is transmitted over serial lines between devices where a single serial cable connecting the serial ports on two devices namely a client and a server.Works on a client/server architecture where slaves/server supply requested data to the master/client. A slave is any peripheral device like RTUs, I/O modules,etc. which processes info and sends it to the master.A master's query will consist of the slave address (slave ID or Unit ID), a function code, any required data and an error checking field. Slaves do not initiate messages and only respond to requests made by the master. Uses specific function codes to call different commands.

* *Modbus(TCP)*- Uses the same request/reply model like Modbus(RTU). It runs on ethernet which is faster and easier to troubleshoot. The error checking field used in Modbus RTU is eliminated as the TCP/IP link layer uses its checksum methods, eliminating the need for the Modbus RTU checksum(this function helps in checking the accurate delivery of the packet). Modbus TCP utilizes the reserved port 502(this port is reserved for modbus applications, helps in listening and receiving Modbus data) to communicate over TCP/IP.

* Both of the above mentioned protocol have a data limit of 253 bytes.

(b) **DNP3 (Distributed Network Protocol 3.0)**- Developed by Westronic. This protocol is used in automation and control of various industries like electric, oil, wastewater, gas utilities because it is resistant to EMI-induced distortion(distortion of the voltage and current waveforms in the power grid caused by external electromagnetic fields), works reliably over varied and low-quality media and can address 65k devices in a single link, supports multiple data types. The data link layer of DNP3 communication has start bytes, length, control, destination, source and CRC (cyclic redundancy check) error checking.

* Key differences between DNP3 and MODBUS protocol
1) *Application*: Modbus is designed mostly for communication between devices in a single master-slave configuration while DNP3 is designed for communictaion in a distributed network of devices.</br>
 
2) *Message Structure*: Modbus uses a simple message structure consisting of function codes and data, while DNP3 uses a more complex message structure that includes more information about data types, timestamps, and event notification.</br>
 
3) *Security*: DNP3 includes built-in security features such as encryption and authentication, while Modbus does not have native security features and relies on external mechanisms for security.</br>

4) Unlinke the MODBUS protocol where the slave does not send any data to the master DNP# can send in an unsolicited response to the master.</br>

5) report by exception(RBE). SCADA server polls for change events.</br>

6) has defined other layers including application,transport and data link layers.</br>

(c) **Profibus(Process Fieldbus)**- It is a field bus communication protocol used to connect, exchange data between various devices in a process conrol system and are inter-operable. Here all the devices follow a proper sequence to connect to a network, each slave maintains a timer. The slave goes into a state known as a safe state if the master does not talk to a particular slave at the right time. If the master wants to exchange data, it has to go through the start-up sequence again.</br>

*Types of PROFIBUS*</br>
~PROFIBUS FMS- initial PROFIBUS protocol which is very simple but was not robust enough to work on complex networks.</br>

~PROFIBUS DP(Decentralised Periphery)-most common,simpler and faster than other protocols, supports the transmissionof data in various cycles such as cyclic,acyclic and isochronous slave-slave mode and data exchange.</br>

~PROFIBUS PA(Process Automation)-standardises the process of transmitting measured data.</br>

(d) **PROFINET(Process Field Net)**- is an open standard for industrial automation designed for scalability, uses etherent to exchange data.</br>

[reference](https://www.sciencedirect.com/science/article/pii/S0167404822004205)



