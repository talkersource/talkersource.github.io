---
title: NUTS
family: nuts
---

{% assign nuts_faq = site.info | where: "key", "nuts-faq" | first %}
## [{{ nuts_faq.title }}]({{ nuts_faq.url }})<br/>

Written by Neil Robertson (neil@ogham.demon.co.uk)

## License

On July 18, 2002, in the `alt.talkers` Usenet group, author Neil Robertson
[retroactively applied][nuts-gpl] the [GNU General Public License v2.0][gplv2]
to all original NUTS source code releases.  (Note: the GPL version was not explicitly
stated but, based on the date, GPLv2 is assumed since it was the latest version
available at the time.)

> I've decided to GPL the entire NUTS code from the very first version to the very last.
> Since I can't be arsed to re-release all the code with a new copyright this post will
> have to suffice. Why anyone would want to use 10 year old badly written flaky code in
> their own I'm not sure but someone did and asked if he could GPL is so I thought what
> the hell, might as well GPL the whole lot.

Presumably, the terms of the GPL license would apply to new derivative works based off
of the original NUTS code after that date, but forks and other derivative works that
already existed as of July 2002 (and also their derivatives, if any) would be
grandfathered under the previous terms of use.  However, this paragraph is not
legal advice; you are encouraged to seek proper legal counsel if you have questions
regarding the full implications of this retroactive assignment.

[nuts-gpl]: https://groups.google.com/forum/#!msg/alt.talkers/1XcZfT_xYwY/i4kc20Rw6C4J
[gplv2]: https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html

## NUTS History (also written by Neil)

NUTS started out as a university project in 1992 for the final year of my
degree course and it was the 2nd best option in my opinion from writing a MUD
which the CS department decided "wasn't appropriate". So I came up with
some specious title for a talker project along the lines of a "multiuser
realtime networked conferencing system" or some such bullshit and they
fell for it :) Having seen a number of other systems such as the complex
EW-TOO by Simon Marsh (which to me seemed to be inhabiting some middle ground 
between mud and talker), the very simple such as the talker built into Unaxcess
(sp?) and the truly appalling (did someone say IRC?) I designed NUTS as being 
a system that anyone would be able to master straight away the minute they 
logged in. These days its somewhat more complex and probably sits alongside 
EW-TOO in the talker stakes but hopefully its still just as easy to use for 
first timers.

These are the dates on which various nuts version were release as best I can
remember or find out...

<style type="text/css">
  #versionlist tr td:first-child { text-align: right; white-space: nowrap; }
  #versionlist thead { font-weight: bold; text-decoration: underline; }
</style>
<table id="versionlist">
  <thead><tr><td>Date</td><td>Version</td><td>Notes</td></tr></thead>
  <tbody>
    <tr><td>Winter 1992</td><td>Chat Server</td><td>Original project code - never released</td></tr>
    <tr><td>Jan or Feb 1993</td><td><strong>1.0.0</strong></td><td>Project code with bug fixes and name change</td></tr>
    <tr><td>?</td><td>1.0.1</td><td></td></tr>
    <tr><td></td><td>1.0.2</td><td>March/April maybe</td></tr>
    <tr><td>May 1993</td><td>1.0.3</td><td></td></tr>
    <tr><td>October 1993</td><td>1.1.0</td><td></td></tr>
    <tr><td>December 1993</td><td>1.2.0</td><td></td></tr>
    <tr><td>?</td><td>1.3.0</td><td></td></tr>
    <tr><td></td><td>1.3.1</td><td></td></tr>
    <tr><td>April 1994</td><td>1.3.2</td><td></td></tr>
    <tr><td>May 1994</td><td>1.3.3</td><td></td></tr>
    <tr><td></td><td>1.3.4</td><td></td></tr>

    <tr><td>June 1994</td><td><strong>2.0.0</strong></td><td></td></tr>
    <tr><td></td><td>2.0.1</td><td></td></tr>
    <tr><td>July 1994</td><td>2.0.2</td><td></td></tr>
    <tr><td></td><td>2.0.3</td><td></td></tr>
    <tr><td>August 1994</td><td>2.1.0</td><td></td></tr>
    <tr><td>September 1994</td><td>2.1.1</td><td>(date from archived tarball)</td></tr>
    <tr><td>November 1994</td><td>2.2.0</td><td></td></tr>
    <tr><td>December 1994</td><td>2.2.1</td><td></td></tr>
    <tr><td>January 1995</td><td>2.3.0</td><td></td></tr>

    <tr><td>Feb 1996</td><td><strong>3.0.0a</strong></td><td>alpha test release</td></tr>
    <tr><td>March 1996</td><td>3.0.0</td><td></td></tr>
    <tr><td>April 1996</td><td>3.1.0</td><td></td></tr>
    <tr><td></td><td>3.1.1</td><td></td></tr>
    <tr><td>May 1996</td><td>3.1.2</td><td></td></tr>
    <tr><td>July 1996</td><td>3.2.0</td><td></td></tr>
    <tr><td></td><td>3.2.1</td><td></td></tr>
    <tr><td>September 1996</td><td>3.3.0</td><td></td></tr>
    <tr><td>October 1996</td><td>3.3.1</td><td></td></tr>
    <tr><td>November 1996</td><td>3.3.2</td><td></td></tr>
    <tr><td></td><td>3.3.3</td><td>Final NUTS 3 version</td></tr>

    <tr><td>September 2005</td><td><strong>4-1.4.1</strong></td><td>(date from archived tarball)</td></tr>
  </tbody>
</table>
