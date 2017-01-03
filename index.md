---
title: TalkerSource.com
layout: root
---

## What are <q>talkers</q>?

{% assign talker_info = site.info | where: "key", "talker" | first %}
{{ talker_info.excerpt }}

[&raquo; read more]({{ talker_info.url }})

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
{% assign codes_by_family = site.codebases | group_by: "family" | sort: "name" %}
{% for family in codes_by_family %}{% assign fam = site.family | where: "family", family.name | first %}
  <h3><a href="{{fam.url}}">{{ fam.title }}</a> family</h3>
  {%for codebase in family.items %}<a href="{{codebase.url}}">{{codebase.title}}</a>{% endfor %}
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
