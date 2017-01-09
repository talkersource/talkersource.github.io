---
key: about
title: About TalkerSource.com
created: 2017-01-09 01:26:44 UTC
updated: 2017-01-09 02:09:56 UTC
---

This site's goal is to maintain an archive of as many talker and related codebases as we can find, to
preserve a piece of the Internet's first purely social ecosystems, before instant messaging and social
media took over.  While we can archive the source code, we cannot recover the friendships that were lost
as servers went offline, one by one.

<!--more-->

{% assign nuts3 = site.codebases | where: "key", "nuts3" | first %}
{% assign tos4 = site.codebases | where: "key", "tos4" | first %}

My name is William (online and IRL), and I joined the talker scene late in its life, around 1997.
I was on my way to becoming a decent spod, and I gained wiz privileges on a few sites before I decided
to try my hand at writing talker code as a means to self-learn the C programming language.  I started
with a copy of [NUTS 3.3.3]({{ nuts3.url }}) and eventually released several minor versions of
[TalkerOS]({{ tos4.url }}). I was honored it found a spot on Neil's [talker family tree][tree] while
he still maintained it and posted to the `alt.talkers.programming` Usenet group, but I was a
relatively _minor_ player compared to most others mentioned on that tree.  I still relied on the
generosity of others for hosting the TalkerOS code, website, and my own little-used talker; eventually
these went away, like many others, in the early to mid 2000s.  Though I was saddened, my contribution
was relatively small and still lived on _somewhere_ on the Internet -- I thought.  Then, sometime in
2009, I realized that I had lost my backup copies of TalkerOS.

For purely nostalgic reasons, I searched the Internet for a copy, expecting to find source code
mirrors on talker-related sites.  I found a copy, but only the latest version, and in the process
of searching I discovered that `talker.com` was shutting down.  This was a _big deal_; talkers had
always been a niche, and in decline as newer Internet communication formats became popular, but this
news was a wake-up call.  I searched for other codebases; there were signs, too, that the "usual places"
to get talker code were rotting, slowly breaking over time.  The Web page might be online, but the
the source code -- often on a separate FTP server -- was no longer available.

Beyond the previous two paragraphs describing the origin of this site, `TalkerSource.com` is not
about any one person or codebase.  This archive is the result of countless Google searches for different
keywords, code names, author handles (and their IRL names); recursive retrieval of entire FTP directories;
snapshots of content found in the [Internet Archive][archive-org]; and, thankfully, a few contributions
from previous spods that stumbled upon the site.

Much of the content hosted and curated by this archive _is not the original work_ of the archive's
maintainer(s).  Credit is given and sources are referenced and linked, on a best effort basis, when the
archive borrows or rephrases stories, histories, and descriptions found within the source code or from
other Web sites.  It is hoped that the source code and Web site authors will see the value of this
archive as a centralized location, much like a museum, for information on the topic of _talkers_.  It has
not been possible to seek advance and express permission in all cases; many e-mail addresses are broken
or are not actively checked by their owners.  Some code is released with clear license terms for distribution
and some not so much. Please [contact the archive maintainers][gh-issues] if you hold the legitimate rights
to one or more works in the archive and have concerns or objections regarding their inclusion here.

[tree]: /talkertree.txt
[archive-org]: https://archive.org/
[gh-issues]: https://github.com/talkersource/talkersource.github.io/issues/new
