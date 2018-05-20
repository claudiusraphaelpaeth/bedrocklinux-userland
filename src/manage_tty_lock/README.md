manage_tty_lock
===============

Set/unset the locks on a given terminal.

Usage
-----

To lock a terminal, use `lock` as the first argument.  To unlock one, use
`unlock` as the first argument.  The second argument can be utilized to specify
which terminal to lock/unlock; if it is left unset, the current terminal is
utilized.

Example, locking /dev/pts/1:

    manage_stty_lock lock /dev/pts/1

Example, unlocking the current terminal:

    Example: manage_stty_lock unlock

Installation
------------

Bedrock Linux should be distributed with a script which handles installation,
but just in case:

To compile, run

    make

To install into installdir, run

    make prefix=<installdir> install

To clean up, like usual:

    make uninstall

And finally, to remove it, run:

    make prefix=<installdir> uninstall
