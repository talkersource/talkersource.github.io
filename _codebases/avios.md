---
key: avios
title: Avios
author: Neil Robertson
github_url: https://github.com/talkersource/avios
family: other
---

AVIOS stands for **A VI**rtual **O**perating **S**ystem, that is it loads and runs multiple
processes written in the AviosPL language which can interact with each other and the outside
world just as in a real OS.

<!--more-->

The main reason for Avios existing is not simply to have a virtual OS, as by itself this
concept isn't that usefull. Its raison d'etre is that it provides a way for people with no C
experience to set up an internet server (or even mulitple ones) and then only having to code
in AviosPL which is a far simpler language than C as well as not having to worry about socket
coding details.

This program only runs on Unix systems. As of writing its been tested on

- HP-UX 10.01 & 10.2
- Linux 1.2.13
- Digital Unix 3.2 (OSF)
- SunOS 5.5

&mdash; Neil Robertson, August 1997

{% assign nuts_family = site.family | where: "family", "nuts" | first %}
See also: [{{ nuts_family.title }}]({{ nuts_family.url }})
