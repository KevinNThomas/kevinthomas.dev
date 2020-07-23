---
layout: post
title: How To Install And Run Ableton Live 10 On Debian Linux
excerpt_separator:  <!--more-->
tags:
 - music
 - wine
 - msitools
 - debian
---

There are a few caveats to installing and running Ableton Live 10 on Linux, and I initially
had some issues getting it working on Debian that I couldn't find solutions for online. Here's
how I got it working:

1. Download Ableton Live 10 (Windows 64 Bit) from Ableton's website
2. Extract the zip file
3. You should now see a file called `Setup.msi`. Wine doesn't work with msi files, you'll need to
install the package `msitools` to work with msi files: `sudo apt install msitools`
4. Normally, to install an msi file, you would run `msiexec /i Setup.msi`, however, that wasn't working
for me. It would just run for a few seconds then finish with no output or results. Instead, run the
msiextract command: `msiextract Setup.msi`
5. You should now see two folders: `Ableton` and `System64`. You can move these two folders to wherever
you want Ableton to be installed
6. To run Ableton, use wine with a 64 bit prefix to run the Ableton exe file:
`WINEPREFIX=/path/to/wine64prefix wine Ableton/Live\ 10\ Suite/Program/Ableton\ Live\ 10\ Suite.exe`
7. Ableton should now be up and running!

Note: Online authorization probably won't work. Follow Ableton's instructions for offline authorization
to get your copy of Ableton authorized.

