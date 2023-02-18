---
key: talkernode
title: TalkerNode
description: A NUTS-style talker base, written in Node.js
author: Marcos Torres (Mind Booster Noori)
github_url: https://github.com/talkersource/TalkerNode
upstream_url: https://github.com/marado/TalkerNode
license: Unlicense
license_note: (a public domain dedication, see unlicense.org)
family: other
---

{% assign nutsFamily = site.family | where: "family", "nuts" | first %}
{% assign mamnuts = site.codebases | where: "key", "mamnuts" | first %}
{% assign pytalker = site.codebases | where: "key", "pytalker" | first %}

TalkerNode was started by the same author who forked [_{{ mamnuts.title }}_]({{ mamnuts.url }})
and later created [_{{ pytalker.title }}_]({{ pytalker.url }}). All behave in the style of 
[{{ nutsFamily.title }}-family]({{ nutsFamily.url }}) talkers, but TalkerNode uses the JavaScript
language and is not derived from the original NUTS source code in C.
