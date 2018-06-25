---
core_id: "4"
title: Security work at Linaro
description: |-
    The Linaro Security Working Group (SWG) mission is to support Arm Open Source Linux distributions on security related topics.
keywords: OP-TEE, TEE, Arm, Arm-Trusted-Firmware, GlobalPlatform
permalink: /engineering/core/security/
principal-engineer: Joakim Bech
related_projects:
  - "5"
related_initiatives:
  - "9"
youtube_playlist: https://www.youtube.com/playlist?list=PLKZSArYQptsOuFyjUlWFWUulxXOhhtsEf&playnext=1
image:
  featured: true
  path: /assets/images/blog/meltdown-spectre-download-linaro.jpg
  name: meltdown-spectre-download-linaro.jpg  
---
# Security
The Linaro Security Working Group (SWG) was created to help ensure an optimised
and efficient software ecosystem exists to support Arm Open Source Linux
distributions on security related topics, and to accelerate the delivery of high
quality secure products across the Arm Open Source ecosystem. The team’s mission
is to avoid and prevent fragmentation of implementations underpinning security
within Arm based systems.

In order to enable secure boot and to enable security on devices one has several
choices to make depending on what architectural layer you are working with. The
SWG are doing work in both normal user space applications as well as
implementing drivers and adding general security enhancements to Linux kernel.
Another area where SWG spends a lot of time is in the so called Trusted
Execution Environment (TEE). Find out more about Linaro's work on OP-TEE on this [website](/initiatives/op-tee/) or on the project's own [domain](https://www.op-tee.org/).

The SWG is creating reference designs showing how normal and Trusted Application
code and libraries can be integrated within a particular platform such as
Android. Activities include the development of an Open Source reference
implementation of the W3C Encrypted Media Extension (EME) using platform
security features for secure media playback on mobile and digital home devices;
and an Open Source reference implementation of secure boot for the 64-bit Arm
Cortex-A series processor cores to complement the Arm Trusted Firmware open
source project, targeted at server applications.

By delivering tested reference Open Source software Linaro will enable SoC
vendors, OEMs and application developers to more easily understand how to design
and build secure applications across a wide range of Arm products and segments.
These include the Internet of Things, mobile devices, the digital home.

### Objective
- Key player in software related to security such as TEE solutions and kernel
  hardening on Arm systems.
- Stabilize Armv7-A and Armv8-A TEE solution(s) running on Android.
- Active role in open sourcing a TEE.
- Active part of Linaro’s (LHG) mission creating DRM/EME reference.
  implementations for Android and Comcast RDK.
- Kernel hardening - with Arm contribution in [Kernel Self Protection Project].
- Include, [Travis], LAVA and CI in the all tasks.
- Actively monitor and contribute to relevant Open Source projects.
- Deliver the Linaro [Open Source Security Project](/projects/open-source-security/)

### Process
The Security Working Group does all planning and tracking in
[JIRA] which you can follow in detail if you are a Linaro member and have the required access
(Linaro IT gives access).

- [JIRA Security roadmap] (password required): https://cards.linaro.org/secure/StructureBoard.jspa?s=138
- [Kernel Self Protection Project](https://kernsec.org/wiki/index.php/Kernel_Self_Protection_Project): https://kernsec.org/wiki/index.php/Kernel_Self_Protection_Project
- [Travis](https://travis-ci.org/OP-TEE): https://travis-ci.org/OP-TEE


*****

# Downloads and help for Meltdown and Spectre
## Open Source Projects
#### Arm
* General Spectre & Meltdown information from Arm, please see: https://developer.arm.com/support/security-update
* Trusted Firmware has a separate security advisories page, please see here: https://github.com/Arm-software/arm-trusted-firmware/wiki/Arm-Trusted-Firmware-Security-Advisory-TFV-6

#### Kernel
The current status for LTS otherwise is that aarch64 backport exists and have
been accepted for kernel v4.9 and v4.14. For arm32 we are waiting for the
changes to be developed and then we will do the backporting.

* Kernel Page Table Isolation: https://en.wikipedia.org/wiki/Kernel_page-table_isolation
* Linaro tree with work in progress: https://git.linaro.org/kernel/speculation-fixes-staging.git
* For more information about the upstream status, please follow the link above in the "Arm" section that takes you to their security-update page.

#### OP-TEE
* OP-TEE has a separate security advisories page, please see here: https://www.op-tee.org/security-advisories/

Page updated: 2018-04-25
