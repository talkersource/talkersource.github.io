---
title: TalkerSource.com
layout: root
---

## What are/were <q>talkers</q>?

Talkers, as they were known, were text-based real-time chat servers that existed on the Internet
during the <q>early days</q> of the public Internet.  This was a time when...

- _instant messaging_ (e.g. ICQ, AOL IM, etc.) did not exist
- the most common Internet access was through work or a university
- home users relied upon very slow _dial-up modems_ that tied up a landline telephone circuit
- a TCP/IP stack (required for Internet communication) was not a standard part of Windows or Mac OS
- _graphical_ Web-browsing was a recent invention; most Internet services were _text-based_

Individual talkers were often customized around a _theme_, and consisted of multiple named
<q>rooms</q> that fit within the theme.  Some rooms were public, and others could be made private
for sensitive conversations.  As the name suggests, the purpose was primarily to enable casual
conversation.  (Unlike MUDs, which were similar software services of the era, but these often focused
more on role- or game-play than conversation.)  Since all communication was text-based, it was relatively
quick (as long as your connection didn't experience _lag_) but mostly required users to be
online simultaneously, in stark contrast to other Internet communication formats such as e-mail or Usenet.
Customizations and distinguishing features, made to attract users to a particular talker server over another,
were almost always applied by changing the source code and recompiling.  Popular code bases were shared
and [forked, renamed, and shared][tree] again.

IRC (Internet Relay Chat) is another text-based, real-time chat technology from the same era and its user
experience exists essentially unchanged on the Internet of today.  IRC networks facilitate chat, messaging,
and even file transfers, but lack the theming that gave each Talker site a unique personality.

[tree]: talkertree.txt

## The Decline

Talkers rapidly declined in both popularity and in the number of operating sites since the late 1990s.
When `talker.com`, a site dedicated specifically to hosting Talker servers, closed in the late
2000s, the mere existence of Talkers was threatened more than ever.  Understandably, as the talker
instances disappear so does their customized source code.  By 2010, nearly all of the original distribution
sources for the most popular Talker code bases (forks) had disappeared, lost to <q>the great bit bucket
in the sky</q>.

## The TalkerSource.com Goal

Our goal is to maintain an archive of as many Talker and MUD code bases as we can find, to preserve a
piece of the Internet social communities that started it all, before instant messaging and social media
took over.  While we can archive the source code, we cannot recover the friendships that were lost as
servers went offline, one by one.

## Talker Codebases by Family

<style type="text/css">
#codebase_index { padding-bottom: 1em; }
#codebase_index > h3 { padding-top: 1em; }
#codebase_index > h3:first-child { padding-top: 0; }
#codebase_index > a { display: inline-block; margin-left: 2.5em; min-width: 6em; }
</style>
<div id="codebase_index">
{% for family in site.family %}
<h3><a href="{{family.url}}">{{ family.title }}</a> family</h3>
{% for cb in site.codebases %}
{% capture cb_family_id %}/family/{{ cb.family }}{% endcapture %}
{% if cb_family_id == family.id %}
<a href="{{cb.url}}">{{cb.title}}</a>
{% endif %}
{% endfor %}
{% endfor %}
</div>

-----

### Looking for more?

This archive project started too late to save them all.  But if you find a tarball of classic
Talker or MUD source code on that backup tape, Zip drive, or floppy diskette, we want to
archive it here!

New submissions, or comments/requests from code authors already included here, can reach
us by [opening an issue on GitHub][gh-issue].

[gh-issue]: https://github.com/talkersource/talkersource.github.io/issues

<p style="font-size: 9pt;">
  An earlier version of this site hosted source code in <a href="https://www.mercurial-scm.org/">Mercurial</a> repositories,
  <a href="http://hg.talkersource.com/" title="Old talkersource.com Hg repositories">available here</a> while supplies last.
</p>
