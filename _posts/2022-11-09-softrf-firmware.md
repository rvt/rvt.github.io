---
layout: post
title: Stratux SoftRF configuration
subtitle: How to configure your SoftRF device for stratux using the Stratux specific version
gh-repo: rvt/SoftRF
_gh-badge: [star, fork, follow]
tags: [Stratux, SoftRF]
comments: false
---

Configuring your Soft-RF Device

**How to configure SoftRF for Stratux**

When you use the modified version of SoftRF for Stratux as found [github.com/rvt/SoftRF](https://github.com/rvt/SoftRF), Stratux
will take care of the configuration using the correct Aircraft ID. However, when Stratux is not beable to modify the Aircraft ID 
of your SoftRF device, for example when you connect over wireless there are two options to configure:

### 1) Connect over USB/Serial on Stratux ### 

When you are not sure how to configure use a terminal and/or send commands to your SoftRF device, you can also for a *one-time* 
connect SoftRF over USB/Serial. Like a T-Beam for example and boot up stratux with the correct Aircraft ID. 
Wait a few minutes, SoftRF will reboot when it received a new configuration from Stratux. 
After the reboot and you see the correct ID you can disconnect and reconnect over wireless again.

### 2) Connect over USB/Serial PC ### 

If you cannot connect the device to Stratux, you can also connect the device to your PC/Mac. I assume you know how to do this so
I won't device to deep in it, I use Arduino. This is also a *one-time* setup.

Use the following link to generate an *$PSRFC* string: [basic.html](/basic.html). Use
the generate *$PSRFC* string and copy/paste it into the device. Here is an example how that might look like:

![SoftRF Config](/assets/blogimg/SoftRF-PSRFC.jpg)

- For explanation of all the settings go here: [SoftRF/wiki/Settings](https://github.com/lyusupov/SoftRF/wiki/Settings)
- For any questions you can find us here : [gitter.im/SoftRF-open/community](https://gitter.im/SoftRF-open/community)
