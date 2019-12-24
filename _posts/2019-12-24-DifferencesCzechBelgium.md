---
layout: post
title: Studying IT - Differences between Belgium and Czech Republic
---

First of all, my best wishes for 2020! May it be a great year where all your wishes may become true.  

In this post I'll discuss my experiences during my stay in Czech Republic. I'll discuss some differences between Czech Republic and Belgium I experienced in school.

## Introduction

This year I chose to study in Czech Republic with the Erasmus Project. VSB TUO is a partner of HOGENT in Belgium and they offer the ability to study a semester in their school. I was able to choose some subjects. I chose all the subjects in the Telecom faculty and my curriculum in Czech Republic become as shown below:

* Advanced Network Technologies
* Practice in Communication Networks II
* Access Networks
* Czech language for foreigners
* VoIP

## Linux, Linux, Linux.

Microsoft Windows is still the standard in our school. All the public workstations on our school in Belgium run on Microsoft Windows. From PC's used in classes to PC's used for printing on the copiers in the library. Also, almost all students use Microsoft Windows on their laptop, a minority uses macOS and almost nobody uses Linux. Here, it is completely different. Public workstations run Debian. They used to say that the compatibility between Linux and printers is often difficult, but people here use the Debian workstations to print because it doesn't work well on Windows...  

Also almost all Czech students in Telecom are using a Linux distro. And after using it for a semester, I have to be honest that I like it very much. My experiences with Windows were not always very good, but I am a mac user so I don't have recent experiences.

## Labs!

One of the major advantages here were the labs. In our school in Belgium we have one network lab, and we are pretty proud about it. It is filled with Cisco routers and Cisco switches and there are separate tables with network connected to the racks and power outlets. 

But, here the labs are completely different. The racks are filled with rack servers, Cisco routers, Cisco switches, Juniper switches, Mikrotik switches, Mikrotik routers, Cisco firewalls and Huawei routers. And while I was there they were upgrading because Mikrotik had some new products.  

Besides that, the most interesting part was that there were 16 desktops in the lab. Yes, desktops. And in my opinion this is a very huge advantage. The desktop runs with a clean installation of Ubuntu 18.04 pre-configured with a hostname and so on, so a clean pre-configured machine. When you reboot the machine, the configuration was only stored in RAM so the machine boots again with a clean pre-configured OS. This is great for testing and you don't have to worry about hypervisors, virtual machines, RAM or anything else. And wen you configured something wrong and you're in trouble, just reboot the PC and you can start again.  

## IPv6

When I attended my first class of 'Practice in Communication Networks II' the teacher told me "This is a Linux and IPv6 only class". The Linux part was fine for me but IPv6??? In Belgium we mostly skipped the IPv6 parts, or they said it is just the same as IPv4. The Cisco Packet Tracer and physical labs were also IPv4 only. So, I had to be introduced to IPv6 again. Of course we learned the basics, but we almost never used it in a real environment.  

I'm very happy I experienced it, we saw the need for IPv6 and it is really time to wake up. Also interesting is that our connection to the Internet was only IPv6. And yes, most of the Internet does not work... Even GitHub is IPv4 only!  

In Eastern Europe IPv6 is already a thing. There are providers that provide only IPv6 public addresses and support IPv4 by encapsulating the packets in a IPv6 packet. So, you have no IPv4 public address anymore.  

When I'm home, I'll definitely dive deeper into it and enable it on my home network. This is very advantageous because you don't have to rely on NAT anymore and you can use the same port for multiple machines.  

The only disadvantage is when you need to connect to your IPv6 machines and you're in a IPv4-only environment. For example on our school last year we didn't have a IPv6 address. Maybe it's already changed but i doubt it. Also the website of our school is not IPv6-enabled because we couldn't visit it in the lab :wink:

## Networking - not vendor locked

The networking part was also very interesting. We learned about technologies that are used in ISP networks. Technologies like MPLS VPN and QOS, Traffic Shaping, Traffic Controlling,... We were also able to implement them on the physicial devices in the lab. Here, they never work with Packet Tracer because they want to give you a real-life experience.  

In the basic network courses (I took Advanced) they also use Cisco courses, but the labs are not given in a Cisco environment. The vision here is that you need to be able to understand the global networking rules and not the one's on Cisco. So they start implementing them on open-source Linux routers. After that they also do some Cisco labs but you can also choose to test the environment on other vendors like Mikrotik.  

The labs are published on the learning managent systems in the Linux environment and the Cisco environment. When you're able to apply them in these two environments, the other vendors are just syntax changes.  

I think this is a good way to learn networking and it's maybe time to think about the fact that Network classes are too vendor locked? Cisco gives lots of discount for schools and academies, but it's maybe not the best way to start learning networking... Stuff to think about :smile:

## Telecom

I also took one course about Access Networks. This was completely new for me because this is not included in my curriculum in Belgium. It was interesting because we were able to take some labs were we could simulate a real xDSL provider. In the rack there were ADSL+ and VDSL2 DSLAMs where we could create some connections. In between we could connect a simulator to simulate distances and measure the impact of the distance on the connection quality.  

This is interesting for use - Belgian citizens - as DSL is an important technology in our country. My Spanish, Polish and Latvian friends were laughing with me because I have no fiber at home, but it's the truth. We're investing so much money in new DSL and COAX technologies instead of investing in fiber. But, we can't do anything about it so it's great to have some knowledge about it.  

Besides DSL we also had an introduction in optical communications, COAX DOCSIS technologies, PLCs, Internet of Things (LoRA, Sigfox, BLE, Zigbee,...), so my general knowledge about these technologies has expanded a bit. And that's always great news!

## The price for studying

Another great difference is the price to study. In Belgium, subscription fees are around 1000 EUR. He're it's a great difference. Studying in Czech Rebpublic for Czech citizens is... FREE!  

But only for state schools. In comparison with the USA state schools are more qualitative than private schools. The only fees are the one's for your books, accomodation and food at school :wink:  

## Open Source

The last thing I'll discuss is the software they're using. Of course if Linux is the first choice, the software choice is a little bit more limited. Every software package I used in the last months at/for school was open source. If they're discussing a specific software package that's commercial our paid, they always have a back-up that's open source and free. And that's also the one we're using. 

For example the web-mail client they're using is Roundcube, the cloud storage for teachers is Owncloud, the office suite on the PC's from school is LibreOffice and so on. 

Also presentations have to be online. And not a Google Slides or Powerpoint Online presentation but a real HTML based one. Most of the students create a website but I chose to use RevealJS. We have a template online in Belgium for our school and I changed it a little bit (the color scheme, the school logo,...). We have to upload it on a VPS we got from the university. Every demonstration of presentation has to be presented on this server. I like this way of thinking :wink:

## Conclusion

It was a great experience. Also very interesting to see the differences between these two countries. They are both member of the European Union but are still so different. I like how progressive the country is. Certainly on the technologic aspect. While Google Pay and Apple Pay are still rare in our country, it's completely normal here. Same in the networking aspect with IPv6.  

I have to say I like the way they're thinking here. If I'll switch to Linux? Partly yes, partly no. Besides IT I'm also occupied in the creative sector (music, photography, video-editing) and the software I use is mac-only. Next year it is almost certain that I'll study music so switching now is a bad idea :wink:. I also like to use a macOS/Apple hardware, I can rely on it (didn't have this experience with Windows), it's fast and durable. My Macbook Pro was second hand from 2014 and still runs like a new one. My Windows-friends already switched in this time-period because it broke or was just too slow.  

If I'll ever use a desktop just for writing, IT stuff and so on (not for the creative software), I'll definitely use Linux on it. Also a big advantage is that it doesn't need lots of resources so a second hand cheap desktop will do the job. 

With regard to IPv6, I'll definitely look into it. The only problem is the other side of the network (which I'll use to connect to my network) but using both IPv6 and IPv4 is also no problem.  

So as you can guess, I loved Czech Republic in many different ways. But I'm also happy to return to Belgium to see my friends and family again. After 5 months I'd be happy to see them again.