---
layout: post
title: Home Server Setup
excerpt_separator:  <!--more-->
tags:
 - home server
 - self hosted
 - docker
---

### I Got My First Home Server Up And Running

For the past few months, I've been interested in switching from a lot of the proprietary
cloud services I use to self hosted free and open source alternatives. Back in late June,
after a lot of research, I finally bought my first home server to accomplish this. Here's
what I got:

* Dell Poweredge R220
* Intel Xeon E3-1240 V3 8M Cache 3.40 GHz Quad Core (Eight Threads)
* 4x 4gb 10600E DDR3 Memory
* H310 Raid Controller
* 2x Brand New 1TB SAS Hard Drives

I bought this server used from Ebay, and got the new hard drives from Newegg (I didn't know
how old the drives that came with the server were, so I wanted to get new ones).

### Configuration

* OS: Debian 10 (Buster)
* Raid 1 Configuration using the H310 Raid Controller
* All hosted services are running in Docker containers

### Services I'm Currently Hosting

* Airsonic - music streaming
* Kanboard - kanban board for project management
* This website - nginx webserver, built-in letsencrypt client, and fail2ban
* Two minecraft servers
* Two mumble servers
* Nextcloud - file hosting
* Photoprism - photo hosting
* Portainer - docker dashboard
* Wireguard - VPN

### Thoughts

Overall this has been a very fun experience. It took *a lot* of setup, research, trial and error,
and troubleshooting, but I'm now at a point where all of these services are working great for me
(well, almost all of them, I currently have an open issue on GitHub for Photoprism).
My skills in server management, Docker, routing, Debian, and security have
all increased a huge amount in the last month, so that has been very rewarding. I'm always looking for
new useful services to self host, so I'm sure this list will grow over time.