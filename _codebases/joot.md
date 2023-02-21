---
key: joot
title: JOOT
description: The Java-based Object-Oriented Talker
author: Dave Jarvis
license: MIT
license_note: (formerly proprietary, non-distributable)
family: other
parent: oot
github_url: https://github.com/talkersource/joot
---

JOOT was notable not only because it was written in Java 1.1 but because its
_source code_ was **not available** to users (without payment). Additionally,
commercial licensing of the compiled binaries was available for a fee.
The following prices are from 1998:

- non-commercial, non-profit and/or educational use: FREE
- commercial use (binaries only): $250 CAD
- source code: $10,000 CAD

Under the original license terms (re)distribution was not permitted, so the copies of
JOOT obtained for the archive contain only the compiled Java `*.class` files (compiled
JVM bytecode), and the _original_ source files may be lost forever. This archive contacted
Mr. Jarvis in early 2023 and obtained approval to preserve JOOT's files in GitHub under
the terms of the **MIT** open source license.

Then and now, author Dave Jarvis requests that you link to his website if you use this
software; since `joot.com` no longer exists as it was, he requests you link to
[`dave.autonoma.ca`](https://dave.autonoma.ca/) instead. Links within the archived files
have been updated similarly, where possible.

The following content is borrowed from the [original `joot.com` website][archive-org-joot-com-98], circa 1998.

[archive-org-joot-com-98]: https://web.archive.org/web/19980111035300/http://joot.com/about.html

----------

### What is JOOT?

JOOT, standing for **Java-based Object-Oriented Talker**, is a real-time, text-based Internet chat server.

JOOT runs on most Unix operating systems, MacOS, OS/2, Windows NT/95/3.1, and any platform that has
a Java Virtual Machine (or JVM for short).

There are two requirements to JOOT:

1. You need a JVM installed on the computer (server) you wish to run JOOT.
2. In order to access JOOT from the Web (in addition to telnet), JOOT must be
   running on the same computer that runs the Web server.

The second condition does not have to be met in order to fully use JOOT.

<a name="applet"></a>[_archivist note: Web-based access relied upon Java Applet technology
that is no longer supported by modern browsers._]

### Why use JOOT?

- It's _fast_, _friendly_, and _fun_
- Easy to configure; most changes are done while connected
- Has help on every command (add your own and/or change the defaults)
- History of over 3 years
- No special software needed to connect
- People may log on _from the Web_[*](#applet)
- Usable by _any_ computer with Internet access
- Uses open Internet Standards

### Features JOOT already has:

- Change over 400 strings while online (`.string`)
- Change major configuration options while online (`.config`)
- Add/Remove/Rename levels while online (`.levels`)
- Add/Remove/Rename/Join/Detatch rooms while online (`.build`)
- Delete users that haven't been on in a given number of days (`.purge`)
- Find out real user ID of the people currently online (`.finger`)
- Read the mail you sent to other people (`.rmail sent`)
- Shows both IP and DNS (`.site`)
- More control over room settings (`.rset`)
- Extended help files (such as `.help set alias`)
- Better editor for user/room profiles (`.information`)
- Send ASCII pictures to a user (`.ptell`)
- Send ASCII pictures to everybody in the current room (`.picture`)
- Ability to link your JOOT talker with other JOOT talkers (`.link`)
- Grant/Revoke commands from users (`.grant`, `.revoke`)
- More `.set` features
- Over 85 more commands
- Multiple commands per macro
- Run multiple talkers simultaneously
- Cumulative logon time
- Encryption for passwords, smail, and message boards
- 14 glorious colours, plus two random
- No hampering limits on the length of user names, room names, tells, etc.
- Multi-threaded commands
- Intelligent macros
- Add new commands, without shutting down
- Set your own Wizard level
- Sorted macros, rooms, and users
- _... and much more!_
