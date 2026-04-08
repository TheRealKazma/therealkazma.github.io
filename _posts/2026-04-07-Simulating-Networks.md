---
title: "Simulating Networks"
excerpt_separator: <!--more-->
date: 2026-04-08 11:37:00 -0500
categories: [Projects]
tags: ccna # TAG names should always be lowercase
---

Through my time at Ozarks Tech I had to take 2 of the 3 CCNA classes that they offer as I decided I wanted to get my associates in cybersecurity. So, I have had my fair share of Cisco's Packet Tracer which is their own in house network simulating software which would probably be fine to be able to study and then take the CCNA. However, I want to be able simulate more than just simple network traffic. This is why I am setting up GNS3 for both my studies in CCNA and for further studies in my cybersecurity journey. See more about that on [Building a SOC]({{ site.baseurl }}{% link _posts/2026-04-07-Building-a-SOC.md %})
<!--more-->

## The Setup

When it comes to setting up GNS3 you mainly have 2 options, baremetal or virtual machine (VM). Given my need for wanting to keep my everyday computers free of extra processes I opted to install it to a VM on my home server. The install process however was quite interesting, as typically I just download an operating system and then install it as normal. The creators of GNS actually offer a .ova file which is a prepackaged vm which contains all the information the hypervisor needs to set it up. However, there was just one problem. They didn't offer a prepackaged file for Proxmox which is what I currently have running on my home server. So, I followed a tutorial online about how to extract a .ova file and then using the disected components I then imported the VM to Proxmox. Once imported the setup process went smoothly got the client installed and configured with the servers configuration. I was now able to create projects, import appliances, and start simulating my networks.

On the next update of this project I will go though what resources I'm using to study for my CCNA exam and how GNS3 helps or improves upon the idea of Cisco's Packet Tracer.
