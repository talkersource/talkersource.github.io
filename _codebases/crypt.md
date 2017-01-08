---
key: crypt
title: CryptMCS
description: The Crypt Multiline Chat System
author: Bryan McPhail, Scott McKenzie & Marty Greenwell
github_url: https://github.com/talkersource/crypt-mcs
family: nuts
parent: nuts3
parent_version: 3.2.1
---

A notable feature of _Crypt_ was its ability to compile and run on versions of Microsoft
Windows (95/NT4) common in its era -- something practically unheard of in the Talker space,
making this a very unique codebase.

The archive contains two branches; the default `master` branch contains one version of the
source code, which consists only of the `*.c` and `*.h` main program files.  Other files
required for actually running a talker are missing from the ZIP file received from the
original author.  Presumably one could use the same file tree from NUTS 3.2.1, but the
archive maintainers have not verified this.  The `rick-collette/6.x` branch contains a
more complete, and newer version of this codebase; it was retrieved from his
[sourceforge.net project][sf] but contains code not written by Crypt's original author(s).

Robert Collette [wrote][sf-news]:

> A long time ago, in a State far far away, I tried to compile a chat system called Crypt
> on my Windows NT 4.0 box using MS VC++ 5. I'm not sure what happened, I think I gave up
> and started hacking the Crypt and messing with it on a linux box I had. Recently I had
> the urge to play with a project, and ran across a MAME hacker who was the guy behind the
> Crypt Talker. I sent him an out of the blue email, asking for permission to continue the
> project on Sourceforge, and get things rolling again. Here's what he said:
>
>> This is the source that used to be on the webpage, plus the unreleased source of the most
>> recent version. Feel free to stick em on sourceforge (let me have the link though!).
>>
>> Bryan

Bryan McPhail [wrote](http://www.bryanmcphail.com/wp/?p=235):

> If I remember right Borland C++ was needed to compile it for Windows NT/95, standard GCC
> was ok for all Unix platforms.

[sf]: https://sourceforge.net/projects/crypttalker/
[sf-news]: https://sourceforge.net/p/crypttalker/news/2005/10/the-crypt-talker/
