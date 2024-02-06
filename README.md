# Introduction

This repository contains images, scripts and notes to build a Debian
image with Iontra gateway, gateway client, aws connector and
associated dependencies. This is a temporary step to create a suitable image for hardware
bringup of phobos large. 

This repo does not use "ansible" and other associated methods used by
the provisioning team. Note that once the provisioning step is
modified to create an image for phytec board with ansible etc, this
repo should be considered obsolete.

# Relevant JIRA/Confluence pages

[INF-959](https://iontra.atlassian.net/browse/INF-959)
[PL-102](https://iontra.atlassian.net/browse/PL-102)
[DELTA-2041](https://iontra.atlassian.net/browse/DELTA-2041)

# Process

We have a base debian image without any iontra software on it called
disk.img.xz. This is stored in git LFS.

We will mount this image and copy gateway and cli client cross
compiled in the host computer.
