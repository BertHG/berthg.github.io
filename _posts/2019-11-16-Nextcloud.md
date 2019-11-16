---
layout: post
title: Nextcloud
---
The plan is to write on a regular time some information about open-source projects I use on a daily basis. The first one I'll discuss is Nextcloud. Nextcloud is an open-source cloud environment that offers so much more than just file storage and file sharing. It's a perfect alternative for the Google suite.

# What is Nextcloud

We're living in a time where everyone uses cloud services. We're using Google Drive, OneDrive, Dropbox,... But are they secure, can we trust them? 

Google knows a lot about us. We do our searches with Google, our calendar is there, maybe your emails? So, do they really need all our documents, photos? Maybe it's time to get our privacy back. Maybe it's time to take control of our documents, photos, etc.  

But which service are we going to use? Well, maybe you should consider Nextcloud. Nextcloud is an open-source service that offers a cloud environment with file storage/sharing and so much more. You can't really take a Nextcloud subscription. Some companies offer Nextcloud subscriptions, but it's more interesting to host your own instance. 

Maybe Nextcloud remembers you of the name Owncloud. In fact Nextcloud is a fork of Owncloud, but now it's much more updated than Owncloud.

Hosting an own instance gives full control over your cloud service. You configure the data limits, the ability to create office documents, sharing, appearance,...

# Features

The features of Nextcloud are almost endless. It goes way beyond file storage and sharing. And besides the files in a webbrowser, you can also access your data via FTP, Windows Network Drive, SharePoint, NFS, object storage and more. 

You can also install some add-ons in Nextcloud. For example Collabora Office (an alternative to Google Docs, Google Sheets, Google Slides,...), a music player, a PDF reader,... There's also Nextcloud Talk, a self hosted VOIP and chat solution.

# Security

Of course security is important. The drawback of hosting your own instance is that you are responsible for the security of your instance. Out of the box Nextcloud delivers some security options:

* Nextcloud has built in monitoring and logging tools
* Administrators can set permissions on sharing and access to file susing groups.
* You can define rules for data retention, allowing regular cleanup of files or ensurances that data stays put for a set amount of time
* File access control: For example XLSX files from the HR department are not to be accessible outside company IP ranges. Everything is configurable
* Multi-layered encryption: Nextcloud uses industry-standard SSL/TLS encryption for data in transfer. Aditionally, data at rest in storage can be encrypted using a default military grade AES-256 encryption with server-based or custom key management. Also optionally and on a per-folder base data can be end-to-end encrypted.

Of course default security measurements should be taken (firewall,...) but this is up to you as you are responsible for your instance.

# Is it difficult?

No, it is not difficult to set up a Nextcloud instance. In fact, there are some options to make it even more easy. There is an official Docker image, so if you are comfortable by using Docker, you can spin up your Nextcloud instance in a few minutes. The docker image is available on the [Docker Hub](https://hub.docker.com/_/nextcloud/).

Canonical and the Nextcloud community maintain a Nextcloud Snap, including release channels. So, if you are a Ubuntu user, you can install Nextcloud by using `sudo snap install nextcloud`.

# What hardware do I need?

## Set it up at home or in colocation

There are two options to host your own instance. You can opt to set it up at home or in colocation. There are no insuperable hardware requirements. Nextcloud is even supported on a Raspberry Pi (it is not recommended). If you search a decent home-server to host Nextcloud on with the ability to set up a software raid, I can recommend the HP Microservers. They are not quite expensive and are very decent.

## Use a dedicated or virtual private server

If you don't like to host the server at home or in colocation, you can opt to rent a dedicated or virtual private server. There are some advantages such as you aren't responsible for possible power outages, network outages, you don't have to keep an eye on the S.M.A.R.T. hard drive statistics,... If you have SSH access to the server, you can set everything remotely up.  

If you're searching for a dedicated or virtual private server for a decent price, you certainly have to take a look at [Serverhunter](https://www.serverhunter.com/?search=9B2-ADB-D24). This website combines server offers from lots of websites and there is a handy filter you can apply to find the server that suits you the best. 