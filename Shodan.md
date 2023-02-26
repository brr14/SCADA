# SHODAN
It is a search engine which helps users discover and access internet connected devices and systems.
Shodan uses a variety of scanning techniques to gather information about devices and systems, including open ports, installed software, and other network characteristics. This information is then organized and made searchable through Shodan's web interface. One of the key features of shodan is its ability to find vulnerable devices with weak passwords that may be at risk of hacking or other malicious activity which can be exploitable by hackers.

## Using Shodan
After gathering a basic idea on shodan I visited Matherly's [website](www.shodan.io) and started to explore it with the help of this [article](https://www.hackers-arise.com/post/2016/06/22/using-shodan-the-worlds-most-dangerous-search-engine). I started off with going to the explore page and searching for web cams which popped up the banner information of many web cams available on the internet. One interesting thing was that they were sorted under various categories like some of them were from the same organisation or some were in the same city which was easier to sort out the data based on what was needed. I got a pictorial view of the places from which the web cams were being accesed on the world maps, further information like ports, operating systems, was also provided.It also displayed some tags which were significant to that particular organisation.

I tried using another tag called *Server SQ-WEBCAM* which led me to various webcams all over the world so I tried getting into one of the webcam server and it worked I got into one of the administration panel of a sever where i could see the different toggles that could move the camera face and more things like change resolution, change size,etc.

I used another tag *webcamxp* which led me many cameras one of which was on a random street of Roanoke in the US.
![ss](/home/roopa/Downloads/shodan webcam.png)

This was a very interesting task I will look into it's uses in SCADA systems next.
