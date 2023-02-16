---
title: "Install AppImage"
date: 2023-02-17T03:10:16+11:00
draft: false
description : "Installing AppImage on your Linux System."
subtitle : ""
header_img : ""
thumbnails : ""
short : false
toc : true
tags : ["Linux", "appImage", "Software", "Install"]
categories : ["Linux"]
series : []
comment : true
---

AppImage is a software Distribution format for Linux. It is getting popular these days for the following reasons:

## Why to use AppImage?

1. Easy To Use
    AppImages are self Contained software. There is no need to install any dependencies or libraries. This makes installation process easier and faster.

2. Portable
    They can run on Multiple Linux Distribution without modification and without compatibility issue.

3. Secure
    AppImages are read only. It cannot edit the system outside its directory. This reduces the risk of malware or other security issues.

4. Convenient
    Can be downloaded and run with single click without any administrative privileges or installation.

5. Versatile
    It can be used to distributed as Graphical or Command Line applications.

## How To Integrate on System

1. Download the appImage file
2. Download icon for your app
3. Copy Both files it on folder /home/user/folder/
4. Right click on the appImage file,
5. click Permission
6. Check ‘Allow executing file as program’
7. Create a text File

   ```
    [Desktop Entry]
    Type=Application
    Name=Minecraft
    Comment=Minecraft
    Icon=/home/user/folder/Minecraft/icon.png
    Exec=/home/user/folder/Minecraft/minecraft
    Terminal=false
    Categories=Minecraft;game
    ```

    > :bulb: **Tip:** Here Icon is place of your icon and Exec is location of your application. We are using Minecraft as example here. Replace these with your folder and file names.

8. Save file in `.local/share/applications/appName.desktop`
9. Save as .desktop format.
10. Log Out or Restart System.

And now you can run your appImage as usual application without problem.