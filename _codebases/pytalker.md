---
key: pytalker
title: PyTalker
description: A NUTS-like talker base, written in Python
author: Marcos Torres (Mind Booster Noori), Daniel Alexandre (FX), José Martins (Hellraiser), Rich Daley (OwlOfDoom)
github_url: https://github.com/talkersource/pytalker
upstream_url: https://github.com/marado/pytalker
license: GPL-2.0
family: nuts
---

{% assign mamnuts = site.codebases | where: "key", "mamnuts" | first %}
{% assign talkernode = site.codebases | where: "key", "talkernode" | first %}

> PyTalker is quite quite dead. This isn't even PyTalker's latest version, or a
> version at all, this is a development snapshot of what almost came to be
> PyTalker 0.3.0 (but never really did anyway).
>
> -- from README

PyTalker was started by the same author who forked [_{{ mamnuts.title }}_]({{ mamnuts.url }}) and
would later create [_{{ talkernode.title }}_]({{ talkernode.url }}). All are in the NUTS family in
terms of behavior, but PyTalker's use of Python is distinct from the NUTS original source code in C.
