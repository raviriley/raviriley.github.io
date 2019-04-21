---
layout: single
title:  "Setting Up Windows for Jekyll"
date:   2019-04-20 16:20:00 -0800
categories: tutorial
---

This is a tutorial for Windows users on how to set up for development of a static site generated with Jekyll. 

**Note**: if you don't know if your system type, go to System Information and check System Type. x64 is 64 bit and x86 is 32 bit. You will need to know this information.

## Install Git
<https://git-scm.com/downloads> - default download settings

## Install Chocolatey
we could manually install everything but Chocolately is a package manager for Windows that does it all for us (big good)

Run one of the following in either Command Prompt or Windows Powershell (your choice):

**PowerShell**:
~~~
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
~~~~

**CMD**:
~~~
@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
~~~~

**Note**: these are both *one line of code*

Now, open a Git Bash command line window and enter:

`choco install ruby -y`

Let that finish & close the window, then open a new Git Bash window and run

`choco upgrade ruby`

## Install MSYS2
Now, we need to install MSYS2, a building tool for Windows with a built in package manager called Pacman. This is used when compiling Ruby gems and is needed to install Jekyll. Run the following from the Git Bash command line:

`choco install msys2`

Once the installation is complete, run

`choco upgrade msys2`

Next, open an MSYS2 window (search for MSYS2 in the start menu - it may be called "MSYS2 mingGW [64 or 32]-bit" or similar) and run the following: 

`pacman -Sy pacman`

if prompted `Proceed with installation? [Y/n]` type Y and hit enter.

Then, open CMD and type:

`ridk install`

3 options should appear - choose `MSYS2 and MINGW development toolchain` - this should be option 3, in which case you type in 3 and hit enter.

If this fails, run the following:

`pacman -S base-devel mingw-w64-i686-toolchain` for 32-bit

`pacman -S base-devel mingw-w64-x86_64-toolchain` for 64-bit

this will run manual installation.

## Setting up Jekyll
enter the following in Git Bash:

`gem install jekyll` 

`gem install jekyll bundler`

You are now ready to create your first Jekyll website!

Before creating your first site, it is recommended you create a folder to store all the jekyll sites you make in one place. This is helpful when pushing to GitHub and hosting on GitHub Pages or similar. 

Head over to the [official Jekyll website](https://jekyllrb.com/) to learn more about Jekyll and how it works. 
Jekyll is written in Ruby, so if you're new to Ruby click [here](https://jekyllrb.com/docs/ruby-101/) to learn about some terminology you will need to know.

[Quickstart Instructions](https://jekyllrb.com/docs/) - get up and running locally in 3 lines of code

**Note**: this will take you to the Jekyll documentation. Use the links in the table of contents on the right of the page to learn more about how to use Jekyll.










