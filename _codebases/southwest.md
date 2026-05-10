---
key: southwest
title: SouthWest
description: "The only true Windows talker server"
author: Scott Lloyd
license: Public Limited (Copyright retained)
github_url: https://github.com/talkersource/SouthWest
family: nuts
parent: nuts3
---

The SouthWest codebase is a talker server written in _Visual Basic 6_ for the
Microsoft Windows operating system.  It was inspired by Neil's Unix Talk Server
(NUTS).  Included in at least version 1.0.0 was an HTTP server that runs on a
separate port.

Talkers in the 1990s weren't known for their security, but SouthWest has the
(in)distinction of having been the subject of [CVE-2002-0496][CVE-2002-0496],
reported on 26 March, 2002, and described by [Internet Security Systems][iss-8626]:

> SouthWest version 1.0.0 is vulnerable to a denial of service attack. A remote
> attacker could send a specially-crafted HTTP request to the HTTP server
> listening on port 5002 to cause the service to crash. The service must be
> restarted to regain normal functionality.

[CVE-2002-0496]: https://www.cve.org/CVERecord?id=CVE-2002-0496
[iss-8626]: https://web.archive.org/web/20030309064836/http://www.iss.net/security_center/static/8626.php
