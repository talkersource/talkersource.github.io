---
key: mamnuts
title: Mamnuts
author: Marcos Daniel Marado Torres (Mind Booster Noori)
website: http://mamnuts.blogspot.com/
github_url: https://github.com/talkersource/mamnuts
family: nuts
parent: amnuts
parent_version: unknown; CVS circa November 2005
---

{% assign pytalker = site.codebases | where: "key", "pytalker" | first %}
{% assign talkernode = site.codebases | where: "key", "talkernode" | first %}

The author of Mamnuts later went on to develop [_{{ pytalker.title }}_]({{ pytalker.url }})
and [_{{ talkernode.title }}_]({{ talkernode.url }}), both in the NUTS family in behavior
but not based on the NUTS source code.
