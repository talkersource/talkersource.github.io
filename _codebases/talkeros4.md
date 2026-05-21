---
key: tos4
title: TalkerOS 4.x
author: William Price
github_url: https://github.com/talkersource/tos4
family: nuts
parent: nuts3
parent_version: 3.3.3
---

On its surface, TalkerOS was a basic NUTS 3 clone.  Its focus was to build
a codebase that was easier to modify for beginners with less coding experience,
and to add support for newer technologies such as the [Pueblo/UE client][pueblo-chaco]
for Windows.

Its notable features included:

### Embedded pictures and audio

Chaco's _Pueblo/UE_ MUD and Talker client supported inline display of still
images (JPEG) and embedding audio (WAV, MIDI) inside a normal Telnet text
stream.  The talker could send special HTML-like markup, after detecting the
client, to instruct it to download and display or play files from HTTP URLs.
Existing or special text elements could be turned into hyperlinks to allow
the user to, for example, navigate by clicking room exits instead of typing
commands.

One command loaded and displayed a picture (given an HTTP URL), which proved
quite popular with some _adult_ talkers.  Another could play a (MIDI) song
from a "jukebox".  All image and song files had to be publicly accessible
for users' clients to download, and files were hosted using other HTTP
servers, not streamed from the talker itself.


### Talker "Firewall"

Though not really a _firewall_ in the truest sense, security and account
takeover was a concern in the late 90s when there were dozens of talkers
(with their owners) hosted on the same server.  Each talker owner usually
had a separate shell account, but sometimes an account's files could be
read by other shell accounts.

When enabled, accounts over a certain level threshold must be listed in the
source code (and compiled) or else an adverse action -- such as an automatic
disconnection -- would occur.  Each account could be associated with up to
two(2) IP addresses or domain names, and if used from a different address
then access could be temporarily limited.


### "Plugin" API and architecture

Talker modifications were traditionally performed by directly modifying the
core code.  This meant that one person's enhancements were difficult to
extract and translate to another talker, even when all parties were cooperating
rather than "stealing".

TalkerOS defined a C function naming and calling convention to allow small
snippets of functionality -- usually in the form of one or more commands -- to
"hook" into the talker with minimal modifications to the core code files.  The
API supported events fired when a user was loaded (after signing in) and also
when user files were saved (usually upon logout), in addition to regular system
"heartbeats".

Sharing commands was made easier, though adding or removing a "plugin" still
required minor code modification and recompiling the talker.

## Development timeline

<!-- some information gathered from https://web.archive.org/web/20040417083927/http://maddhouse.com/%7Etalkeros/news.html -->
<table id="versionlist">
  <thead><tr><td>Date</td><td>Version</td><td>Notes</td></tr></thead>
  <tbody>
    <tr>
      <td>May 1997</td>
      <td><strong>(unreleased)</strong></td>
      <td>Initial development; hosting courtesy of <tt>snafu.net.au</tt></td>
    </tr>
    <tr><td>?</td><td>pre-4.0</td><td>Offline development, online debugging thanks to &quot;Garth&quot;</td></tr>
    <tr><td>December 1997</td><td></td><td>24/7 hosting on <tt>page.az.net</tt></td></tr>
    <tr><td>?</td><td>4.00</td><td>&quot;Simpler&quot; setup, consolidated color codes; hosting moved to <tt>maddhouse.com</tt></td></tr>
    <tr><td>June 1998</td><td>4.01</td><td>Adds 'plugin' hook architecture, Pueblo multimedia client support, firewall, TalkerBOT, personal rooms, etc.</td></tr>
    <tr><td>October 1998</td><td>4.02</td><td>Bug and stability fixes; MagicEightBall and Poker plugins pre-installed</td></tr>
    <tr><td>March 1999</td><td></td><td>First ideas formed for version 5.0</td></tr>
    <tr><td>June 1999</td><td>4.03</td><td>Security patch for NUTS 3 login flaw</td></tr>
  </tbody>
</table>

-----

{% assign lotos = site.codebases | where: "key", "lotos" | first %}

Chaco Communications later released Pueblo as an [open-source project][pueblo-src].

Parts of TalkerOS were borrowed and integrated into other codebases.
Notably, the Slovakian _[{{lotos.title}}]({{lotos.url}})_ borrowed the
TalkerOS "plugin" API and the Pueblo hyperlinks and multimedia features.

[pueblo-src]: https://sourceforge.net/projects/pueblo/
[pueblo-chaco]: https://web.archive.org/web/19990203125145fw_/http://www.chaco.com/pueblo/index.html
