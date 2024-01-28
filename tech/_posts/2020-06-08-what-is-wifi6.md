---
title: "Why WiFi 6 could be a game changer" 
permalink: /tech/:title
collection: tech
category: tech
date: 2020-06-25
---

Wi-Fi 6 is the consumer friendly name for the IEEE 802.11ax, which is the current generation Wi-Fi specification standard and the successor to Wi-Fi 5, also known as IEEE 802.11ac.

This new standard comes with various improvements to efficiency and throughput. It is also backwards compatible with your older devices since it supports both 2.4 Ghz and 5 Ghz bands.

But, before we can dive deep into explaining what is Wi-Fi 6 and advantages it bring to the table, we need to be on the same page regarding certain terminologies. We shall also setup some analogies that we will use to explain technical details in simpler terms.

To connect to the internet, we will need to install either a modem or gateway provided to us by internet service providers. If it is the former, a router typically is connected to the modem to provide additional connection points such as ethernet ports and Wi-Fi for our devices to connect to in order to access the internet. If a gateway is used instead, the gateway itself is also a router and could also provide the same functionality as a standalone router.

With that in mind, let us imagine the router to be a large warehouse in a middle of a small city. It has a number of gates or main doors that represent antennas. In addition, there are buildings (or clients, if you will), which represents devices such as smartphones and laptops. Then, there are also couriers who represent radio waves. These couriers are the middlemen between the warehouse and the various buildings, and are responsible for transporting packages to the mall and back to their respective clients. These packages contain things, which are pieces of data, that the building need.

### It is fast

Wi-Fi 6 has a theoretical maximum speed of 9.6 Gbps (gigabits per second) or 1.2 gigabyte per seconds. That is almost 2.6 times more than Wi-Fi 5. To put things in perspective, it is possible to transfer a 100GB 4K blu-ray video in just under two minutes with such speed.

There are three key technological updates that contribute to Wi-Fi 6's improved performance over the previous generation: *MU-MIMO*, *OFDMA* and *1024-QAM*

**MU-MIMO**

MU-MIMO stands for "multi-user, multiple input, multiple output". It is a technology that help increase the number of antennas a router has and could be found implemented in most Wave 2 Wi-Fi 5 (IEEE 802.11ac) routers and devices.

Wave 1 Wi-Fi 5 and earlier routers could only communicate with one device one at a time and the others have to wait until it is their turn.

With MU-MIMO release for Wave 2 routers, they could communicate with up to four devices simultaneously.

The caveat here is that, the location of each client device matters. If two or marke devices are in the same general location, they will still need to wait in line to communicate with the router.

And you might wonder how does this technology help to improve performance?

Let us assume that a router will be placed in the center of the house or a room. Then, if there are multiple devices around that require Wi-Fi access, they could access the router via the nearest antenna pointed in their respective general direction. If two or more devices are in the same general location, then these devices will share the same antenna and need to wait for their turn.

For those who have a hard time understanding that, let us go back to the analogy we created earlier.

When the warehouse is first built, which represent the earlier version of Wi-Fi, there is only one gate. In order to enter or exit, couriers need to queue up by the gate and wait for their turn before they can proceed to either deliver or collect their respective packages.

Then, with MU-MIMO technology for Wave 2 Wi-Fi 5, the warehouse undergoes a renovation to have four gates installed according to the points on a compass instead of just the one. Now with four gates, more couriers can enter and exit albeit from four different directions at any given point in time. With this, the buildings are now able to get their requests serviced faster.

But if a particular gate has a long queue of couriers, they will still need to wait for their turn to enter or exit unless they choose to use other gates.

And for Wi-Fi 6, MU-MIMO is upgraded to support up to eight devices at the same time.

Going back to the warehouse example, renovation is done to add four more gates, for a total of eight. More couriers now can enter and exit the warehouse from eight directions at any given point in time, therefore servicing even more buildings.

**OFDMA**

Orthogonal frequency division multiple access (OFDMA)is an extension of Orthogonal frequency division multiplexing (OFDM) technology.

But, before we can dive deeper into OFDMA, we must first understand what is OFDM.

OFDM is a technology that takes a radio channel such as the 20 Mhz channel, which is often used for Wi-Fi, and sets a number of sub-carriers instead of having just one carrier. For Wi-Fi 5, 52 sub-carriers can be created from a single 20 Mhz channel using this technology while Wi-Fi 6 take that to the next level and can create 234 sub-carriers.

To the uninitiated, a carrier is a modulated wave that convey information.

Each sub-carrier is then modulated independently and simultaneously to form symbols, which are waveforms that represent information or data. And these symbols are separated in time by guard intervals to prevent interference cause by neighbouring sub-carriers. Finally, a single transmission to the receiving device will consist of a number of these simultaneous symbols spanning the sub-carriers.

The receiving device is able to track all these sub-carriers simultaneously and extract data from each sub-carrier independently. This contributes to the increase in Wi-Fi performance since multiple pieces of data are transmitted at the same time.

However, the problem with OFDM is that any device is free to transmit a signal whenever they are ready, creating a first-come-first serve situation. This may work in a home-setting where there are not a lot of devices but does not work in a high-density area such as a stadium and shopping mall. Too many devices will be fighting for a chance to send and receive data from the router, resulting in an inefficient use of the router.

For those who have trouble following the above explanation, let us go back to the warehouse example we used earlier.

OFDM can be thought of as multiple couriers who are dispatched to a specific building but at slightly different timings. They travelled on the same road but on a different lane, and each of them carries a different part of the final data. Once they arrived at their destination, the building's manager will collect the different parts of the data and began the reconstruction process. Even if some of the couriers got lost, the manager is still able to reconstruct the data because each courier carries a nice little clipboard containing a detailed description of the content and its relation to the other couriers.

However, there could be couriers serving other buildings traveling on the same road. Some of these couriers could end up on a lane where other couriers are on. This can lead to a scenario where the couriers would fight amongst themselves in order gain access the warehouse first. During the fight, packages will be lost and when that happens, the buildings need to dispatch couriers with the same packages again in an attempt to gain access to the warehouse.

This is where OFDMA comes in.

OFDMA technology solves the network contention issue by grouping the sub-carriers into Resource Units (RU) to service one or more clients depending on their needs.

Therefore, if there is a client that need higher bandwidth because of the data it is downloading, then all the sub-carriers can be grouped as one Resource Unit to give the client the full bandwidth of the channel. Similarly, if multiple clients in the same area need a fraction of the bandwidth because of their small data requirement, then multiple Resource Units can be created to serve all of the clients.

And the change in the RU configuration is also done in real time, therefore enabling a consistent efficient use of the available network bandwidth.

To the layman, it is the equivalent of upgrading the warehouse to dispatch one truck per lane to serve a group of buildings that are close together. The purpose of the truck would be to carry as many couriers as it can hold and transport them to the group of buildings where they could then drop or pick up the packages.

When does the warehouse dispatches the trucks and decides whether the couriers on board all serve the same or different  building are dependent on the requirements such as the service type, package size and total number of packages.

With that, the odds of couriers losing their packages and having to restart the transport process again, which is an overhead, is reduced. Furthermore, the different buildings (clients) in the same area get an equal amount of attention from the warehouse. Furthermore, the different buildings (clients) in the same area get an equal amount of attention from the warehouse.

**1024-QAM**

Wi-Fi 6 improves on the amount of data transmitted per signal, allowing improvement in speed by up to 30%. This means that you can stream bandwidth hungry content such as 4K video with further reduction in loading times and have a smooth viewing experience.

But before we could dive deeper into how Wi-Fi 6 achieve this, we need to understand how Wi-Fi work in general.

Wi-Fi works by using radio waves. To transmit data so that the receiving device understand it, the sender need to modulate the signal to represent bits of binary code. This type of modulation is known as "Quadrature amplitude modulation" or QAM for short.

The better a device is at modulation, the more information it can transmit each time.

For example, a 2-QAM device means it capable of transmitting one bit (1 or 0) of information each time because it can modulate the signal in one of the two ways. A 4-QAM device can transmit 2 bits (00, 01, 10, 11) of information each time because it can modulate a signal four different ways.

With that in mind, current generation of Wi-Fi 5 devices are 256-QAM, which means eight bits of information can be transmitted each time. This is why most of us today do not spend a lot of time waiting for video to load and buffer. With Wi-Fi 6, devices are able to do 1024-QAM, which means 10 bits of information can now be transmitted each time.

To explain QAM much simply, let us go back our warehouse example.

2-QAM is the equivalent of the courier only having one hand. They can either carry one bag or nothing at all. 4-QAM give them another hand, so now they can carry up to two packages. 256-QAM for Wi-Fi 5 is the equivalent of giving a courier four pairs of hands, thereby enabling them to carry up to eight packages. With the upgrade to 1024-QAM for Wi-Fi 6, each courier now has five pairs of hands to carry up to ten packages.

On the surface it may not look like much. However, if a request is for a large amount of data such as those typically found during 4K movie streaming, having the ability to transfer more data per trip will mean less trips needed to download the full content. After all, less trips equals more time saving.

### It could improve battery life

Other than being faster, Wi-Fi 6 also comes with a new feature call Target Wake Time. This allows certified Wi-Fi 6 routers to schedule check-in times with connected devices.

With scheduling, devices only activate their antennas at the right time instead of having to keep their antennas powered on to transmit or search for signals for an extended period of time, which can consume quite a fair amount of power.

For devices such as laptops or desktops which are connected to a power source and do need persistent internet connection, this feature may not be useful. But for IoT devices it could be a world of difference since they may not have access to consistent power and probably run on batteries.

### It has better security

Since 2004, the Wi-Fi security revolves around WPA2. It is a protocol that encrypts the communication session between the router and the client device so that they could exchange information safely and privately.

WPA2 was considered to be very secure until 2017 when a [weakness](https://www.krackattacks.com) in the protocol was discovered that made it possible for attackers in range of the Wi-Fi router to steal sensitive information.

The Wi-Fi Alliance announced WPA3 in 2018 to be the replacement. WPA3 replaces the need for the 4-way handshake to authenticate a client in WPA2 with another method called Simultaneous Authentication of Equals (SAE).

SAE is a proven zero-knowledge method to establish a secret shared key that both the client and the router will use to generate the session key to encrypt and decrypt Wi-Fi transmissions. If another client wishes to connect to the network, the client will established its own secret shared key with the router.

The other important feature of WPA3 is Forward Secrecy, which is an indirect effect of implementing SAE. This ensure that even if an attacker managed to capture the encrypted Wi-Fi transmissions and then crack the session key, older data continue to remain unaccessible as the keys used to encrypt those data will be different.

WPA3 is optional for existing devices and many device manufacturers may choose not to patch these products via firmware update. But in order for these manufacturers to market their devices to be Wi-Fi 6 certified, the Wi-Fi Alliance mandated that WPA3 be implemented. Therefore, we can be sure that Wi-Fi 6 will be more secure.

Other than improvements made to the WPA protocol, the security and privacy of open Wi-Fi networks such as those we find in cafes, shopping malls and stadiums are also improved. Wi-Fi 6 will see the implementation of Opportunistic Wireless Encryption (OWE).

OWE is a security technique that is similar to SAE to encrypt the transmission channel between the device and the router but without the need for authentication. The established shared key is only known to the client device and the router.

Although it is not as secure since there is no way to tell who is connected to what, it is more secure than connecting to a public Wi-Fi secured by WPA2 and using a the pre-shared password, or connecting to a completely open Wi-Fi network.

