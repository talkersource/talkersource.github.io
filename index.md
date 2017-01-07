---
title: TalkerSource.com
layout: root
---

## What are <q>talkers</q>?

{% assign talker_info = site.info | where: "key", "talker" | first %}
{{ talker_info.excerpt }}

[&raquo; read more]({{ talker_info.url }})

## What happened to them?

The first talkers often ran as _unauthorized_ services on university networks, whose unamused administrators
often forced the talker owners scrambling to find alternative hosting sites; in that way, keeping a talker
online was precarious from the start.  Despite this, talkers boomed in the 1990s until they declined in both
popularity and in the number of operating sites at the end of that decade.  Many blame the introduction of
the instant messaging platforms ICQ (1996) and AOL Instant Messenger (1997) for talkers' demise, along with
end-user expectations or preference for modern, _graphical_ systems over "old school" text terminals.

When `talker.com` -- the first and largest site dedicated specifically to hosting talker servers -- closed
in 2009, the continued existence of talkers was threatened more than ever.  Hosting a talker takes time,
effort, and system administrators willing to grant shell access. While many talker site administrators found
homes on other servers, these, too, atrophied and few remain to date. Understandably, as the talker instances
go offline so does their customized source code.  By 2010, nearly all of the original distribution sources
for the most popular Talker code bases (forks) had disappeared, lost to <q>the great bit bucket in the sky</q>.

## Why TalkerSource.com?

{% assign about_us = site.info | where: "key", "about" | first %}
{{ about_us.excerpt }}

[&raquo; read more]({{ about_us.url }})

## Codebases by Talker Family

<style type="text/css">
  #codebase_index { padding-bottom: 1em; }
  #codebase_index > h3 { padding-top: 1em; }
  #codebase_index > h3:first-child { padding-top: 0; }
  #codebase_index > span { display: inline-block; margin-left: 2.5em; margin-bottom: 1em; min-width: 9.5em; }
</style>
<div id="codebase_index">
{% assign codes_by_family = site.codebases | group_by: "family" | sort: "name" %}
{% for family in codes_by_family %}{% assign fam = site.family | where: "family", family.name | first %}
  <h3><a href="{{fam.url}}">{{ fam.title }}</a> family</h3>
  {%for codebase in family.items %}<span><a href="{{codebase.url}}">{{codebase.title}}</a></span>{% endfor %}
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
