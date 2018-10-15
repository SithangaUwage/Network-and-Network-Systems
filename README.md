# Network-and-Network-Systems

![alt text](/Images/KeyTable.png)
![alt text](/Images/IPAddress.png)
![alt text](/Images/Downstairs.png)
![alt text](/Images/Upstairs.png)

Security
The network above for the IoT Smart Home contains three firewalls, a super hub router and a Wi-Fi extender. The super hub router is located downstairs and the Wi-Fi extender is located upstairs, this is done to keep the strength of the signal strong for all the device connected to the network. The created IoT Smart Home network is affordable for the everyday household users and it provides the security needed to keep the data safe within the network to prevent attacks such as DDoS, malicious programs being installed onto the device and to stop cybercriminals from accessing the network.
The network diagram uses a star network topology which is one of the most common network setups. The setup contains a central node and all the other nodes are connected individually to the central node with Ethernet cables as shown by the green connection lines. In the diagram above the central node is the super hub router and the nodes that are connected to the hub are the Wi-Fi extender and the office computer.
There are several number of advantages of using a star network and one of them is that if one of the nodes fails then the others won’t be affected and it will be very easy to find the unresponsive node. If the network needs expanding, then the new nodes just need to be plugged into the central node. However, there are several number of disadvantages of using a star network and the main disadvantage is that if the central node (super hub router) fails then the whole network will fail. The network can be expensive if there are a lot of nodes being connected and the switch must be powerful to accommodate the devices, also the cost of cabling used to connect all the devices to the central hub will add to the cost of the network.
The IoT Smart Home Network will use intrusion prevention system (IPS) firewalls. The IPS sits between the firewall and the network and will examine the flow of the traffic in the network. If malicious activity is presented it will prevent the activity from gaining access to the network. The IPS firewalls will examine both the input and the output of the traffic flow travelling through the super hub and the input of the Wi-Fi extender. A firewall for the output of the Wi-Fi extender won’t be necessary as the traffic would have already be examined by the output firewall of the super hub.
The advantages of using intrusion prevention system is that the system will send an alert to the administrator with details of the type of malicious activity being sent to the network, ending the traffic from the address and resetting the connection. The system works fast to detect and remove the threats while making sure that legitimate packets are not misread as threats. There are two main detection mechanisms used by the IPS the signature based detection and the statistical anomaly based detection.
The signature based detection breaks down into two methods, one being the exploit facing signatures which identifies patterns of exploit attempts and the other being vulnerability facing signatures which targets underlying vulnerabilities in the system that is being targeted. The statistical anomaly detection takes random traffic samples and compare the samples with pre-calculated samples, if the results are outside the baseline then action will be taken by the IPS to handle the situation.    
There are several ways to keep the network secured, one of the most basic protocols to take to secure the network is to change the default password of the router, the name of the router and to create a strong complex Wi-Fi password. This will prevent anyone who is unauthorised to use the network from gaining access. By changing the default manufacture name of the router for e.g. on Virgin router the name begins with VM, it makes it harder for the unauthorised person from trying to access the network from finding out which manufacture has created the router for the network, as there may be certain techniques in which the hacker can use to break into the router. Changing the default password will also make it harder for the attacker to break into the router as the attacker tend to use publicly known credentials to gain access and having a strong complex password will make it difficult for them to crack the password.
Using antivirus software such as Avg, Norton or Mcafee for device connected to the network can prevent virus from being download or becoming a victim to identity theft and spyware. It is important to have antivirus software downloaded on every device that has connectivity to the internet to prevent any of these types of attacks from occurring, as personal data can be easily accessed by unauthorised personal. The attackers may also want to take control of the device for their own gain, such as using them for their botnet armies, so they can launch DDoS attacks.
When browsing the internet use incognito mode, as it protects the user’s privacy and adds security, mainly when the computer is being shared with someone else. Websites that the user’s visits won’t be saved in the browser history and cookies that are created are automatically deleted, so login details and passwords are harder to crack even if the user forgets to sign out of the account.    
Another step to keep the network secure is to update the routers firmware to the newest addition as the manufacture’s makes sure that any security breaches that occur to their products or any vulnerabilities they find are fixed and the shields that prevent the different types of breaches are up and running, so firmware that has not been updated can be breached by hackers and are vulnerable to such attacks.
More advanced security implication can be used to protect the network, such as creating port forwarding rules combined with IP filtering on the router allowing only specific devices outside the network to communicate with other devices on the network and vice versa. This is an application of network address translation (NAT) which is a function inside the router that allow multiple devices in the network to appear to the internet as one device with one address (public IP address). The devices inside the private network will be invisible to the hosts on the internet as they will communicate with a private IP address. In the assessment brief one of the requirements was that the office can be accessed both internally and externally and creating port forwarding rules will allow this to happen. If the user wanted to access the office computer outside the network, one port number can be set aside for exclusive use of communicating with the device inside the private network and the incoming connection with the correct port number will have access to the computer with that address. Changing the configuration of the router may be difficult for some users, so software’s such as UPnP port forwarding can be used instead which automatically sets the router to forward traffic to the allocated port.
IP packet filtering can be used to allow or disallow specific types of IP traffic, so creating many definitions called filters will define for the router which device can send / receive certain data. Identity spoofing also known as IP spoofing is when a hacker masquerades their IP address and gain unauthorised access to computers and networks where the attacker can send data to a computer or a network with a forging IP address indicating that the data is coming from a trusted host. By filtering specific types of IP traffic from outside the network can prevent attack like IP spoofing from occurring.
For the created IoT Smart Home network, the IoT fridge will be allowed to access external networks for ordering food however external networks will be disallowed to access the IoT fridge and any other device in the kitchen. To access the devices in the kitchen, the user must be inside the network, as accessing the device outside the network can be a vulnerability if unauthorised personal get remote access to the devices. These types of rules are created as a security measure, so the devices aren’t being misused. The firewall is the system that block and disallows the specific IP addresses from getting inside the system as it is the first and last line of defense in the network.
The CCTV cameras are connected to a DVR as another security measure, as if the network was to be compromised then the attacker won’t be able to access the camera footage inside the house. This would be the case if the camera’s being used were IP cameras. To access the CCTV footage the user can either log in through the DVR itself or gain access to the system by logging into the CCTV server using a mobile phone or a laptop.    
Disable remote access on the router is another security protocol that can be used to protect the network. As cybercriminals, won’t be able to access the routers private setting from a device that isn't connect to the network. This will prevent them from altering the setting on the router and won’t be able to control the devices inside the networking which prevents attacks like DDoS, Botnet and many others. As the IoT Smart Home is based on the star network topology, if the attacker gets access to the central hub then they would have control of the whole network.
Creating a guest network that is isolated from the main network adds more security to the IoT Smart Home network. If the devices the visitors are connecting to the network are compromised by malicious malware, virus or have a Trojan horse program installed then the main network will not be affected and will prevent any sensitive information from getting into the wrong hands. Also, it is useful to create a guest network to isolate IoT device, if the previous security measures are not in place or the firewall being used doesn’t have the IPS features, as the IoT devices tend to have a low security level. This prevents the devices from having contact will computers which have more sensitive information and personal data can be stolen in the process of the devices be hacked.   
The simplest and easiest ways to protect the IoT devices inside the network is by switching the devices off when they are not being used. Switching the power off prevents anyone or any device from gaining access to that device to steal sensitive information or the devices being used as a botnet for a DDoS attack.
The network diagram created on page one illustrates a cost-effective network setup with security features that will protect the network from unauthorised personal and protect the devices connected from malware and viruses, also ensuring the signal connecting the device and the hub are strong. The network could be improved to full extent however this will be very expensive and in the future if the house was to be sold then the network value will cost more than the house itself.

Network Attacks
Distributed Denial of Service known as DDoS is a cyber-attack used to make an online service unavailable by flooding the network with traffic of junk data. When the attack is taking place, people won't be able to access online information and will disrupt an organisation's online operations. "The attacks are also used as smoke screens to draw attention away from nefarious activities."
Attackers send malicious software through e-mails, websites and social media to infect computers so that they can use the infected computers to build networks, this is known as "botnets". The attackers can control the infected computer remotely without their owners knowing.  The larger the number of infected computers (up to millions of machines) the stronger the DDoS attack.
There are many different forms of DDoS attacks such as the Pings of Death, Nuke, Slowloris and many others. One of the most common attacks is the UDP (User Datagram Protocol) Flood, which send numerous UDP packets to random ports on a remote host. This causes the host to check for the applications associated with the packets and when there is no information related to the packet, the host sends back a "destination unreadable" packet. The attack repeats itself over and over until the system becomes overwhelmed and unresponsive. The attacker will also spoof the IP address off the packets to make sure the attack is anonymous and the ICMP packets don't reach their host. Software’s such as UDP unicorn can be used to perform DDoS attacks and they are commercially available.
DDoS attacks can be bought through the black markets and anyone can pay a fee to silence online services that they don't agree with. An example of these types of services, for "$150 can buy a weeks-long of DDoS attacks on the black market (TrendMicro Research)".
Ping of death, known as PoD attack attempts to send oversized malicious ping packets to a computer system. The maximum packet size a computer system can handle for a IPv4 packet including the header is 65,535 bytes, Ethernet connection packet size is 1500 bytes and amounts that are larger than this size would not be able to be handled by computer systems, causing them to crash, reboot and even freeze. The attackers will split the packet into multiple IP packets known as IP fragments. This will allow the packets to fit the size criteria and later resembling them into the complete malicious oversized IP packets which may overflow the memory and crash the system. The only detail the attacker will need to know is the IP address of the computer they are attacking and they will be able to easily hide their identity, which was why the attacks were so popular.        
To prevent PoD attacks, firewalls can block the internet control message protocol, known as ICPM ping messages however this approach will not hold viable in the long term as blocking ping messages will prevent the user from legitimate ping use. The best option to use in terms of prevents these attacks is to selectively block fragmented ping packets which will allow actual traffic to pass through without hindering the system.
Slowloris developed by Robert Hansem is a DDoS attack which allow a computer to take down a web server by opening multiple connection to the server and keeping the connections open as long as possible. The attack send partial Hypertext Transfer Protocol, HTTP requests which are never completed and the servers will keep the connection open until the connection pool is filled to the maximum capacity, denying legitimate connection made by clients. The slowloris attack can bypass the intrusion detection system without causing any red flags to appear in the system. The attack itself can be slow as the attack must wait for sockets to be released before consuming them. Software such as PyLoris, Goloris and many other can be used to perform the slowloris attack while providing additional functionalities.
To mitigate slowloris attacks connection timeout can be set in place, however making sure the timeout is not too short or long. If the connection is slow between the server and the receiving party, then there will be a risk of dropping the legitimate connection and if the timeout is long then there won’t be any protection from the attack. Another method to use for stopping such attacks is to define the minimum incoming data rate. If the connection is slower than the minimum data rate, then the connection will be dropped.
Botnets are computers that have been infected with malware and are controlled by cybercriminals to perform various attacks, without the knowledge of the user. Botnets can be used to perform DDoS attacks, steal private data and many other illegal activities. Computer system that have low security defenses can be breached by several different ways which allows an attacker to take control over the system. This process is known as the bot recruitment where the bot header will start sending botnet viruses, worms and other malware over the internet in the forms of infected emails or downloads which will breach low defense systems. The infected systems will start to connect back to the attacker’s command and control servers. The larger the number of infected computers, the more damage the attacker can carry out.
Botnets can be used for recording sensitive information like financial data using malware such as Key logger or in the form of Trojan horse like Zeus Botnets. Trojan Horse are programs that infects a computer when it gets inside the system. The programs can be download through e-mail attachments, websites or from file transfers, as the program appears to be legitimate. One of the most common Trojan program's is one that appear to prevent and remove viruses from the user’s computer, however the program is malicious and can steal private information. These types of malware record the keystrokes used for logging into financial account and sends the information to the attacker who can use it for online identity theft, credit card theft or to sell the data collected.
Botnets are largely used in DDoS attack where the attacker uses the infected computer army to bombard victim’s servers with requests, attempting to connect to the server which cause the system to overload and crash. Click fraud is another attack performed by botnets, where the bot computer visits the websites to create false web traffic. The larger the amount of traffic visited onto a site that pays per click, the owners of the websites are paid a large amount of money from the advertisement companies.
Botnets are hard to detect as they are design to operate without the user’s knowledge, however there are few signs that will help the user to find out if their computer system is infected. The first being that there have been connection attempts with known command and control servers. Slow computing or high CPU usage and even problems with internet access will help to detect if the computer system has been infected. To prevent botnet infection several measurements can be placed such as network baselining, software patches and anti-botnet software’s.
Network baselining is where the network activity and the performance gets monitored for irregular behavior. If irregular network activity has been found on the system, high advanced antivirus software can be used to find malware on the computer or by blocking the network connection between the system and the server. Software patches is a term used for keeping all the software up to date within the system itself and the network devices. The latest firmware tends to keep up to date on preventing any new botnet virus and keeps the systems safe. Finally, anti-botnet software such as network sniffers, network intrusion detection systems and many other programs provide botnet detection and removal of the virus without the infection occurring in the system. Botnet detection is useless without botnet removal as the virus tend to work fast to infect the system, so as soon as the program detects the virus it needs to be removed as quickly as possible.             
