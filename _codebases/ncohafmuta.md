---
key: ncohafmuta
title: Ncohafmuta
author: Anthony J. Biacco (Cygnus)
github_url: https://github.com/talkersource/ncohafmuta
family: other
parent: iforms
---

Ncohafmuta is a text-based chat server that is designed for access from a telnet client.
Its purpose is to allow users to communicate in a configurable environment in realtime.
It allows users to create accounts with their own settings and optional personal information.
Rooms are the basis for communication, whether private or public. Other features include
internal email, email forwarding, a configure script for multiple Unices, support for cygwin
under Win32, macros, games, a ranking system with access to more commands, ANSI coloring,
banning, async DNS, soft/hot-rebooting, detailed, organized logging, and an internal Web
server port. 

<!--more-->

&mdash; from [freecode.com][freecode]

-----

According to the [Talker Family Tree][tree], the Ncohafmuta codebase was derived from _Iforms_
which was itself a fork off of [NUTS 1.x][nuts1].  So from that perspective, one could argue that
Ncohafmuta belongs in the [NUTS family][nuts].  However, it is one of only a few codebases -- if
not the _only_ codebase -- actively in-use at the beginning of <q>the decline</q> and still
based off of _NUTS 1.x_.  Most other active NUTS-derived codebases at the time had forked from
Neil's 3.x line, making Ncohafmuta a unique if not original variant.

**Versions**<br/>
1.4.x - stable<br/>
1.5.x - development

**NOTE:** The author maintains a separate [GitHub repository][upstream], which may contain
newer or different changes when compared to this archive's repository.

[tree]: /talkertree.txt
[nuts]: {% assign nuts_fam = site.family | where: "family", "nuts" | first %}{{ nuts_fam.url }}
[nuts1]: {% assign nuts1 = site.codebases | where: "key", "nuts1" | first %}{{ nuts1.url }}
[freecode]: http://freecode.com/projects/ncohafmuta
[upstream]: https://github.com/abiacco/ncohafmuta
