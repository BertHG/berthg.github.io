---
layout: post
title: Visual Studio Code Server
---
Hello, my next post will revolve around Visual Studio Code Server. Visual Studio is very popular these days. And that's right!
Visual Studio Code became my only editor I use. I write all my notes for school in it (Markdown on GitHub), I write my LaTex files in it, I use it to create yaml files for Ansible, I write bash scripts in it, Powershell, Python,...
Also, the great thing is that the terminal is built-in Visual Studio Code. So, it is possible to use vagrant or powershell seamlessly along with your newly created files. And of course, as it is bash (if you're a Linux or macOS user), you can commit, push, merge using this terminal.
The only thing I missed is that it only runs on PC. Now that I am on Erasmus, I carry an iPad with me to make my handwritten notes, to read PDFs and so on (because I don't want all that paper on the plane, and because I'm not a great fan of paper :wink:), but I miss Visual Studio Code on it.
So, of course for every problem ther's a solution. I found out that it is possible to deploy a web-based version of Visual Studio Code on a server.

# Visual Studio Code Server

Microsoft recently introduced Visual Studio Online. This is of course a commercial product of Microsoft with a monthly fee. But, as Visual Studio Code is open-source and the community is rather big, there's someone who created a solution that you can host yourself.

The Github repository of the Visual Studio Code Server can be found [here](https://github.com/cdr/code-server). This is a docker image.

# What about the marketplace?

Of course one of the strengths of Visual Studio Code is the marketplace. I use lots of extensions to make work easier so this is something that is essential. This version does not provide access to the official Microsoft marketplace, but the project created an own marketplace that they manage for open-source extensions. Of course, I don't do rocket-science on the iPad, so I found everything I needed (Live markdown extensions and so on) to get the work done. As I said, I usually just use it to take notes in markdown and push them to my GitHub repos.

# How to install it?

It is possible to use the docker image from cdr (the official author of the project), but I use a fork of Linuxserver (a community who creates docker-images of lots of open-source projects). The image can be found on the [Docker Hub](https://hub.docker.com/r/linuxserver/code-server). So it's really simple. On the command line use `docker pull linuxserver/code-server` to install it. It's not unusual that you want to change some parameters. I refer to the README on the docker hub to change options (for example the port of the service, the volume where you like to store the config files), but everything is clearly explained on the README page.

# Bonus: useful extensions

Here I'd like to share some extensions I use regularly (feel free to drop me an e-mail if you have other recommendations - I'd be happy to add them)

* Angular development: **johnpapa.angular2** (I'm not a professional Angular developer - I just like to play with it from time to time ::wink::)
* Ansible: **vscoss.vscode-ansible** This is the official Ansible extension from Microsoft. It offers Intellisense and useful features to run ansible over ssh
* Arduino: **vsciot-vscode.vscode-arduino**. This is the offical Arduino extension from Microsoft. The main advantage is that you can show the serial monitor in Visual Studio Code and you also have the ability to upload the sketches to Arduino right within VS Code. So, no need to install the Arduino software anymore.
* Cisco IOS: **jamiewoodio.cisco** This is an extension that provides syntax coloring for Cisco scripts. I used it for some labs on my Erasmus where we had to make some IOS scripts. Syntax coloring is always helpful in case of debugging. And that's - yes - almost alwas the case ::wink::
* CSV (and Excel - yeah :satisfied:): **grapecity.gc-excelviewer** A CSV file is not easy to read (OK, I speak for myself), so sometimes it's easier to view the CSV files immediately in table form - right within Visual Studio code. And bonus, it also has support to view Excel files within VS Code...
* HTML: **abusaidm.html-snippets** An extension to support snippets when writing HTML
* LaTex: **james-yu.latex-workshop** An extension with full support for LaTex. It has built-in debugging (which is VERY useful - In TexStudio it was sometimes very hard to find the errors and this helps me more). I also had sometimes issues with the biber support in TexStudio, but with this extension in VS Code I never had issues. As I need to write a lot of LaTex for my bachelor thesis, this is a very useful extension. And again, now everything can be done with 1 editor instead of lots of editors
* Markdown: **yzhang.markdown-all-in-one** This is a dream-extension. It's super easy now to write Markdown files. You can use it just like you used to use Word. When you want something bold just press CTRL/Command+B - Italic: CTRL/Command+I. It automatically adds lines for lists, you can make table of contents,... Everything you ever wanted from Markdown is possible with this plugin
* Paste images: **mushan.vscode-paste-image** If you use Markdown for your notes, this is a must-have extension. You need to press CTRL+SHIFT+P (Linux/Windows) or CMD+SHIFT+P to paste the image that is on your clipboard. Then, it automatically creates a file of the picture in the working-directory and adds the markdown snippet in your file to add the picture in your Markdown file. So, when you're working and you copy a screenshot on your clipboard, you now can directly add the picture to your Markdown file instead of saving-moving,....
* Powershell: **ms-vscode.powershell** I have to admit that I don't want to use it, but I have to :grinning:. This is the extension that adds support for Powershell (Intellisense,...) You can also use it on Linux/macOS if you installed Powershell Core
* Formatting: **esbenp.prettier-vscode** In my opinion the best formatter for every language I use
* Python: **ms-python.python** Official extension for Python made by Microsoft. Offers Intellisense, debugger and so on
* XML: **dotjoshjohnson.xml** Offers a Tree-viewer for XML files. 
* YAML: **redhat.vscode-yaml** Official extension of RedHat. Offers Intellisense and validation.

# Questions

If there are any questions or difficulties while installing, feel free to drop me an email. My e-mail address can be found on the About page. Happy coding in VS Code Server!