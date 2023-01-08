---
layout: page
title: Homelab
permalink: /homelab/
weight: 3
---

# My Homelab

As you may have noticed, this site is not running on some purchased web hosting or VPS, it runs on private server 😱. You may think that I'm another one with Raspberry Pi4 or even 3 and calling it a **PRIVATE SERVER**, but you don't have to worry about this because this stage is long behind me 😅. Let me introduce you to my homelab.

---

{% include elements/figure.html image="/assets/homelab-topology.png" caption="My homelab graph" %}

Every machine in my homelab except Raspberry Pi runs **Docker** with **Portainer** for monitoring, and I use a single `docker-compose.yaml` file to set everything up.

On Dell and HP minipc I use stable Debian 11, but my so called *BigPC* is running Ubuntu Server 22.04 due to requiring newer kernel by Intel 12gen.

I create a backup of every machine on a daily basis around 3AM, and backups are created on a separate drive for more security and "just in case".

Setup shown on the graph is running stable and without any problems for past few months, my plan for upgrades in near future is to add discrete GPU to *BigPC*. I want it to be an Intel ARC because I never used any, and it can be something new and probably challenging, but unfortunately for that I need to wait a bit because Intel ARC requires kernel minimum 6.0 😞.