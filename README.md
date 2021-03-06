MHI
===

mhi is a commandline style mailreader in the tradition of mh and nmh,
but mutated to support IMAP.

[![Build Status](https://travis-ci.org/pjz/mhi.svg?branch=master)](https://travis-ci.org/pjz/mhi)

Why?
----

One thing that IMAP provides is the ability for multiple clients to
access the same mail store. Graphical clients are all well and good,
but sometimes a reversion to the commandline is necessary. Neither mh
nor nmh will talk to an IMAP server (mh's original semantics, which
nmh duplicates, rely on messages not auto-renumbering, as they do in
IMAP folders), so I had to write my own client.  Python's imaplib made this easy.

How?
----

As of v0.6.5 MHI is available as a PyPI package (`pip install mhi`)
The same version also incorporates the old mkLinks wrapper-script functionality
via:

      python -m mhi.mklinks <destdir>

TODO:
-----

 * use click
 * more help - should be self-documenting

Licensing information is in the LICENSE file. (short version: GPLv3 or CCBYSA)

