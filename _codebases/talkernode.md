---
key: talkernode
title: TalkerNode
description: A NUTS-style talker base, written in Node.js
author: Marcos Torres (Mind Booster Noori)
github_url: https://github.com/talkersource/TalkerNode
upstream_url: https://github.com/marado/TalkerNode
license: Unlicense
license_notes: This is a public domain dedication, see: unlicense.org
family: nuts
---

{% assign mamnuts = site.codebases | where: "key", "mamnuts" | first %}
{% assign pytalker = site.codebases | where: "key", "pytalker" | first %}

> PyTalker is quite quite dead. This isn't even PyTalker's latest version, or a
> version at all, this is a development snapshot of what almost came to be
> PyTalker 0.3.0 (but never really did anyway).
>
> -- from README

TalkerNode was started by the same author who forked [_{{ mamnuts.title }}_]({{ mamnuts.url }}),
and later created [_{{ pytalker.title }}_]({{ pytalker.url }}). All are in the NUTS family in
terms of behavior, but TalkerNode's use of the JavaScript language is distinct from the NUTS
original source code in C.
