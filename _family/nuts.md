---
title: NUTS
family: nuts
---

> The following FAQ is transcribed for posterity from the NUTS homepage. It has been formatted
> in the style of this site; you can view the [original text formatting][faq-txt] or
> download it from the [original source][faq-src].

[faq-txt]: nuts-faq.txt
[faq-src]: http://www.ogham.demon.co.uk/nutsfaq.html

-----

## NUTS Frequently Asked Questions v1.1 (26/7/97)

Written by Neil Robertson (neil@ogham.demon.co.uk)

### What is NUTS?

NUTS stands for Neils Unix Talk Server and is a term for a collection of
different versions of server which have been produced over the years since
1993 (all written by me). The current (and final) version is 3.3.3 which was 
released in November 1996. NUTS was born out of a university final year 
networking project which escaped the clutches of my lecturers storage/waste 
bin and made it out onto the internet with the "rm" command snapping at its 
heals to become one of the most popular types of talk server alongside Foothills
and its derivatives.

### Where can I get it from?

The current version is available at the official NUTS site which is:
ftp://ftp.ccs.neu.edu/pub/mud/servers/misc/nuts/nuts333.tar.gz

The only problem with this site is that it can be rather slow but
apparently there are other sites with NUTS on though I've lost my list
and don't know where they are. If anyone cares to remind me...

There is also a web page at: http://www.ogham.demon.co.uk/nuts.html

### How does it work?

All NUTS servers are written in C for unix systems and they use TCP sockets
to set up ports which users connect to to log in on using a client program 
such as Telnet or TUsh. NUTS versions 1 and 2 only supported line mode client
sessions and so ruling out most Windows clients (awwww) but NUTS 3 also
supports character mode so Windows telnet users can also connect (though
this area is still a bit flakey in certain respects such as in echoing).
Anyone with a suitable Unix ANSI C compiler should be able to compile NUTS so
long as they have the required libraries on their system. FreeBSD users note
that there is a problem with the crypt libraries on your system.

### What will it run on?

NUTS is exclusively a Unix program, it will *not* compile or run on any
other system type without a serious amount of recoding. I'd like to see
it running on NT and VMS but I have no access to a development system on
either of these so thats unlikely to happen. As for any other platform, well
are there any that are worth the effort? W95 is too unstable, 3.1 and MacOS
have no pre-emptive multitasking so they're out, no one uses OS/2 and porting
to MS-DOS would be impossible as the required libraries and functionality 
simply aren't available.

### What are the features?

Apart from the usual stuff such as multiple rooms, internal mail, message
boards, user profiles, etc., the latest version of NUTS also supports among
other things: ansi colour, cloning, auto shutdown/reboot and the ability to 
link talkers together via the "netlink" facility.

The netlink facility is really what seperates NUTS 3 from ealier major
releases. Each talker can have as many links as it has rooms as 1 remote
talker is allowed to connect to each room and once a link is established
either via your talker initiating the link or a remote talker doing it, then
users can traverse the link (which appears as a room link) and find themselves
on the remote system. Once they are there then they can behave as a local user 
would on that system the only restrictions being that they cannot use the 
editor and they cannot traverse yet another link to another talker unless it
is a link back to their own home talker.

The cloning facility is only available to wizes and gods (though that can
be altered to suit) and allows them to create clones of themselves in 
particular rooms so they can listen in to the conversation without actually
being there. In effect the wiz can be in a number of rooms at once. An example 
of use would be if a wiz and someone else were in a room having a conversation 
but the wiz also wanted to be in the login room so when someone arrives he can
welcome them. Clones can speak so the wiz can have a cursory chat with the new 
person via his clone. Another use is when the clone is set so it only hears 
swear words (normally it relays all speech in its room back to its owner). A wiz
could create a clone in a room where some known trouble makers are hanging out 
but he would only ever see the parts of the conversation where any abuse is 
occuring (though anyone with half a brain can just spell his swear words 
slightly different so the wiz sees nothing). Basically clones are a bit 
frivolous but I simply wrote them as a programming challenge.

ANSI colour codes are supported and can be placed in speech, mail,
profiles, messages by users as well as being available to be used in the
C code itself by using special NUTS colour codes. Not everyone likes colour
and some terminals don't support it so it can be individually switched off
by a user but in general I think it makes a talker look nicer. After all, if
colour is no big deal why don't we all still watch black and white TV?

### Are there any bugs?

Unfortunately yes. NUTS 3.3.3 is close on 8000 lines of code and the chances
of 1 person (me) being able to find and remove 100% of the bugs is pretty
small. All the bugs emailed to me by other people have been fixed, however the
ones which went unnoticed until it was too late (and some fixes for them) are 
listed on the following web page: 

http://www.ogham.demon.co.uk/nutsbugs.html

### IForms looks like NUTS, what is it?

IForms is a bastardised version of NUTS 1 written by "Deep" (real name Vince
Rohr). Its a semi-rewrite of NUTS 1 and personally I'm not a great fan of 
either its code or its online functionality but some people like it. It's looking
rather dated these days.

### Are there any other hacked NUTS versions?

Yes, loads, though as far as I know they're mostly all one offs created by
the administrators of the talkers using the code. I believe there are or were
a couple of other modified NUTS versions knocking around the net available to
the public but I don't know their names. Please be aware that I will not help 
you fix or modify *any* already modified version of NUTS so if you have one of 
these don't bother mailing me with any problems.

### The future of NUTS

NUTS 3 will not be developed any further unless theres an unprecedented
demand for a bug fixed version. I was planning on doing a NUTS 4 but I
couldn't really see any way to develop NUTS any further without it suffering
from feature bloat. What I am doing instead is writing a virtual OS which
is called Avios (A VIrtual OS, pronounced _avee-os_) and has pre-emptive 
multitasking of processes written in the Avios programming language. The 
system will allow easy building of network servers (eg: a time server requires
3 lines of code) without the user having to resort to coding C or worrying
about socket creation and calls.

-----
