---
title: EW-too
family: ewtoo
---

{% assign cph = site.codebases | where: "key", "cph" | first %}
{% assign ewtoo = site.codebases | where: "key", "ewtoo" | first %}
This family of code all ultimately derived from Simon Marsh's work on the [{{ ewtoo.title }} codebase]({{ ewtoo.url }})
that powered the _Elsewhere II_ talker.  It was modeled from the original _Elsewhere_ talker, which
had inspiration from [_{{ cph.title }}_]({{ cph.url }}) and _Cat Chat_ before it.
