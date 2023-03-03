---
title: "Update All Apps with One Line Of Code in Windows"
date: 2023-03-04T01:39:38+11:00
draft: false
description : "Winget is CLI tool that Installs, Updates and List All softwares on your windows machine, similar to apt-get, brew, pacman, nix, etc"
subtitle : ""
header_img : ""/images/winget.webp"
thumbnails : "/images/winget.webp"
short : false
toc : true
tags : ["Windows", "Softwares", "Winget"]
categories : ["Windows"]
series : []
comment : true
slug: "winget"
---
 

Its a headache to update each softwares on Windows. Its tough to update something manually.
We do not use Microsoft Store, Microsoft. Please Leave us alone. With said that, Microsoft
store do have a very important application there though and we can use that to update any
and everything, well most of it.
[Winget](https://apps.microsoft.com/store/detail/app-installer/9NBLGGH4NNS1)

## Winget

Winget is an Open Source Windows Package Manager designed to run from Command Line Interface (Terminal). From one simple command you can Install your favorite package, uninstall non-necessary ones and Update, those needed to be updated. Also it lists all the package you have installed in your system, and export it. You can format your pc and install all those packages by importing them, or give it to your non tech savvy friends so they can install those cool softwares.

## Let's Dive into it.

To install Winget:

Go To [Winget](https://apps.microsoft.com/store/detail/app-installer/9NBLGGH4NNS1).

It will open Microsoft Store. Click on Get.
Once Installed maybe, restart your pc.

Head straight to terminal and execute following command:

Winget Help
`winget --help`

See winget version
`winget --version`

Find Winget Packages
`winget find vscode`
This will look for vscode in the Packages.
'Id' is very useful here, you may want to copy it.(just select and right click)

Lets install VScode.
`winget install Microsoft.VisualStudioCode` (right click for paste)

So installation is done. Lets see the list,
`winget export -o C:\Path\to\exported.json`

similary to import
`winget import -i C:\Path\to\exported.json`

## Upgrade

To upgrade all available packages:
`winget upgrade --all`
Follow the Prompts and....
Done!

## Wrap Up

- Install winget
- Install, Update and Uninstall from CLI
- Upgrade Everything available with one line