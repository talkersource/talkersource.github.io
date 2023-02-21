---
key: oot
title: OOT
description: The Object-Oriented Talker
author: Dave Jarvis, Ken Savage
license: GPL-2.0
family: other
github_url: https://github.com/talkersource/oot
---

> You'll find that OOT is closer to a hybrid of C++ and C, than it is of
> pure Object-Oriented C++.
> 
> -- OOT README

The archive contains the published version of OOT 1.0 source code, obtained from a
crawled [version of the `joot.com` website][archive-org-joot] courtesy of `archive.org`.
Then and now, author Dave Jarvis requests that you link to his website if you use this
software; since `joot.com` no longer exists as it was, he requests you link to
[`dave.autonoma.ca`](https://dave.autonoma.ca/) instead.

[archive-org-joot]: https://web.archive.org/web/19980111035230/http://joot.com/

## Frequently Asked Questions

(modified slightly from the original `joot.com` website)

- How do I run OOT on a different port?  
  Typing `oot 7000` would run OOT on port 7000.  
  
- How do I give my own account highest access?  
  In OOT, you must create an account, log out, and edit the file `users/username.dat`
  (substitute your alias for "username"). Change the first number in the file to
  at least 4.  
  
- Is OOT based on NUTS?  
  For the most part, no. I took a peek at NUTS to see the symantics of socket
  communication, but wound up going to the books . . . to figure out how sockets work.  
  
- Colour doesn't work!  
  Some telnet clients (like EWAN) have to be told to change their _emulation to ANSI_
  (from something like VT100). This is typically done through an Options or Settings
  menu. Alternatively, clients can connect up to the talker from the Web.  
  [_archivist note: Web connectivity relied upon Java Applet technology no longer
  supported by modern browsers_]  
  
- Why does colour have to be spelled like that?  
  OOT was written by two Canadians. . . The spelling is British.
