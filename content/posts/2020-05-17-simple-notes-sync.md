---
title: A simple note workflow
layout: post
tags: 
- notes
- joplin
- syncthing
date: "2020-05-17"
description: "Note like on Evernote, but keep your data."
---

So, I've decided to set up my own note taking solution using Syncthing and Joplin. It was simple to get going, albeit a bit complicated.

The items you need:  
	- [Joplin](https://joplinapp.org/)  
	- [Syncthing](https://syncthing.net/)  

Step 1: Create a folder in your filesystem for your notes. In my main system, it's on D:\notes.

Step 2: Start Joplin. Under Options > Synchronization, set the Synchronization target to "Filesystem". The path should be pointed to your notes folder.
![Joplin](/assets/joplin.png)
Step 3: Start Syncthing and create a shared folder:  
	- Name: Whatever you want.  
	- Path: Your Notes Folder.  
	- Folder ID: Choose something unique.  
![Folder](/assets/folder.png)
Step 4: Set up a device in Syncthing. Share the notes folder under Sharing.
![Devices](/assets/devices.png)
Step 5: Accept both connect request and share request on the other device.
