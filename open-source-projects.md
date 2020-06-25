---
layout: page
title: Open Source Projects
sidebar_link: true
sidebar_sort_order: 4
---

### debian-gaming-setup

#### Overview
debian-gaming-setup is an interactive shell script for installing recommended tools to game efficiently on the Debian distribution of the Linux operating system. It is licensed under the GNU General Public License (Version 3).

The repository is hosted on my <a href="https://gitlab.com/KevinNThomas/debian-gaming-setup" target="_blank">Gitlab</a>.

#### Features
The script is written in Bash, and guides the user through the installation of the following tools:
* Nvidia or AMD graphics drivers
* Steam - the largest video game digital distribution service for computer games
* Wine - a tool that allows Windows programs to run on Linux
* Lutris - a Linux video game manager

#### Testing
The script uses [Zenity](https://github.com/GNOME/zenity) to provide the option of interacting with the script using GUI dialog boxes, rather than through the terminal.

The script has unit tests written using [Bats (Bash Automated Testing System)](https://github.com/bats-core/bats-core). GitLab's CI tool runs these tests, along with [ShellCheck](https://github.com/koalaman/shellcheck) when code is pushed to the repository.
