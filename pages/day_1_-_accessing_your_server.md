---
title: Day 1 - Accessing your server
---

## INTRO
:PROPERTIES:
:heading: true
:END:
### You should now have a remote server setup running the latest Ubuntu Server LTS (Long Term Support) version. You alone will be administering it. To become a fully-rounded Linux server admin you should become comfortable working with different versions of Linux, but for now Ubuntu is a good choice.
### Once you have reached a level of comfort at the command-line then you'll find your skills transfer not only to all the standard Linux variants, but also to Android, Apple's OSX, OpenBSD, Solaris and IBM AIX. Throughout the course you'll be working on Linux - but in fact most of what is covered is applicable to any system in the "UNIX family" - and the major differences between them are with their graphic user interfaces such as Gnome, Unity, KDE etc - none of which you’ll be using!
### Although there is a "root" user, you will be logging in and working from the user account that you setup. Because this is a member of the group "sudo" it is able to run commands "as root" by preceding them with "sudo".
## YOUR TASKS TODAY:
### LATER Connect and login remotely to your server
:PROPERTIES:
:later: 1604581960597
:END:
### LATER Run a few simple simple commands to check the status of your server
:PROPERTIES:
:later: 1604581964196
:END:
### LATER Change your password
:PROPERTIES:
:later: 1604581966024
:END:
## INSTRUCTIONS
## Remote access used to be done by the simple telnet protocol, but now the much more secure SSH (“Secure SHell) protocol is always used.
## If you're using any Linux or Unix system, including Apple's MacOS, then you can simply open up a "terminal" session and use your command-line ssh client like this:
`ssh user@<ip address>`
## For example:
 `ssh support@192.123.321.99`
## On Linux distributions with a menu you'll typically find the terminal under "Applications menu -> Accessories -> Terminal", "Applications menu -> System -> Terminal" or "Menu -> System -> Terminal Program (Konsole)"- or you can simply search for your terminal application. In many cases Ctrl+Alt+T will also bring up a terminal windows.
## If you have configured the remote server with your SSH public key (see "Password-less SSH login" in the EXTENSION section of this post), then you'll need to point to the location of the private part as proof of identity with the "-i" switch, typically like this:

`ssh -i ~/.ssh/id_rsa support@192.123.321.99`
## A very slick connection process can be setup with the .ssh/config feature - see the "SSH client configuration" link in the EXTENSION section below.
##
