---
key: lotos
title: Lotos
author: Pavol Hluchy (Lotos)
github_url: https://github.com/talkersource/lotos
family: nuts
parent: amnuts
parent_version: 2.2.1
---

{% assign tos4 = site.codebases | where: "key", "tos4" | first %}

An AmNUTS-based, Slovakian codebase that is a mashup of features borrowed from several others
in the archive, including the "plugin" architecture and (uncredited) Pueblo multimedia client
integration from _[{{tos4.title}}]({{tos4.url}})_, as mentioned in the following snippet from
the embedded `manual.txt` (translation by Google Translate):

-----
Lotos is based on the AmNUTS 2.2.1 code by Andrew Collington . . . In addition to the
AmNUTS 2.2.1 code, Lotos uses parts of codes from other NUTS modifications.  Here is a
list of them with a description of which ones were used:

1. TalkerOS 4.03
    - plugin module system
    - this view of the manual
2. Ncohafmuta 1.2.0
    - macro system
    - possibility of using e.g. 'chattering' commands on multiple users at once
    - many pictures
3. Moenuts 1.59
    - talker backup
4. Gaen K 16
    - font system and their use
5. Crypt V5
    - fonts and working with them
6. some supplements from various Slovak talkers
    - Star AMD talker
    - Nook
    - Hysteria - counters
    - MARS talker - restart (reinitialization)
    - Kesican - transport system
