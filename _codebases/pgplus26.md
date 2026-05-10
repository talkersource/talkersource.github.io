---
key: pgplus26
title: Playground Plus 2026
author: Tony Mattke (tonhE), Jeremy Modjeska (Raindog)
website: https://github.com/playground-plus
github_url: https://github.com/talkersource/playground-plus-2026
upstream_url: https://github.com/playground-plus/playground-plus
family: ewtoo
parent: pgplus
---

{% assign pgplus = site.codebases | where: "key", "pgplus" | first %}

This community effort started in 2026 as an effort to keep the PG+ codebase alive by making
it compatible with modern Linux systems and patching security issues.  There is a separate,
and similarly unofficial "companion" [repository][pgplus-patches] of various patches.

Copied from the project's README:

> Playground Plus is a multi-user chat server ("talker") with a rich history stretching
> back to the early 1990s. Originally built on the EW-Too codebase, it evolved through
> Summink and Playground 96 into Playground+, which became one of the most widely deployed
> talker platforms of its era.
>
> This release brings PG+ into the modern age. It builds cleanly on current 64-bit Linux
> systems with zero errors and zero warnings, fixes critical security vulnerabilities, and
> replaces deprecated system APIs - all while preserving the talker experience that
> operators and users know.

The project does not purport to change ownership, copyright, etc., from the original
authors of _{{ pgplus.title }}_:

* Richard Lawrence (Silver)
* J. Bradley Christian (Phypor)
* Jeoffrey Swift (Blimey)

Ed. note: This archive is listing the last known _maintainers_ of the 2026 variant as
the "authors" within the archive metadata.

[pgplus-patches]: https://github.com/playground-plus/playground-plus-patches
