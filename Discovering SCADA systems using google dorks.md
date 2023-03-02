# Discovering SCADA systems using google dorks
* I started off with this google dork:"inurl:/Portal/Portal.mwsl" which is the dork for the Siemens S7 series of PLC controllers which were similar to the ones used in the Stuxnet attack.
It opened up a portal to S7-1200 station_2 / PLC_1</br>

![Screenshot from 2023-03-02 19-57-18](https://user-images.githubusercontent.com/96241263/222457032-7146d893-5327-4ff8-9055-6d2960f8855d.png)

* Now I entered the ip address of the server into Shodan where it showed that it was located in Gabin,Poland. It also displayed the vulnerabilities of the server.
![Screenshot from 2023-03-02 20-05-50](https://user-images.githubusercontent.com/96241263/222458946-a62d8599-ea9c-49be-855b-e57aa6a3eb1b.png)

* On clicking the diagnostics tab we can see the firmware version ,serial number,etc.
![Screenshot from 2023-03-02 20-16-10](https://user-images.githubusercontent.com/96241263/222461620-d8de02ff-87bf-4bc0-830a-67272de1a6af.png)

We can also access the MAC address, netmask(defines range of IP address),etc without logging in.
![Screenshot from 2023-03-02 21-11-49](https://user-images.githubusercontent.com/96241263/222478964-299789f8-b7a1-4572-a65a-53f836e34d82.png)

This was a very interesting tasks as we see how one of the most powerful tools in the industry can be so vulnerable and easily hacked.
