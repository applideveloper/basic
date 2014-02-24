** ** Chipmunk Basic README ** **   (version 3.6.6b0, 2012-Apr) 

Chipmunk Basic is a old-fashioned interpreter for the BASIC
programming language.  This is a beta release of a terminal
command-line utility, and a Carbon window application, for both
for Mac OS X with Intel CPUs and PPC CPUs.

Features of the Mac OS X Carbon window port include support for
simple graphics with a sprite graphics engine, sound, MacinTalk
speech.  It's also AppleScriptable.  A te2cbas AppleScript
is included to run programs from the TextEdit application.
A tw2cbas AppleScript is included to run programs from the
TextWrangler application.

Please see basic.man.txt for documentation of the Basic language.
Please see the quick-ref for Mac specific features.

Use the Terminal utility to run the command-line version (The
Terminal utility is in the Mac OS X Applications / Utilities
folder.)  The command-line executable named "basic" can go into your
/usr/bin directory ( use: sudo mv -i basic /usr/bin/basic ), or any
other directory in your execution $path.  The basic.1 man file goes
into your /usr/share/man/man1/ directory.  Then type "man basic"
to see the man file in readable form.  Note that from the Terminal
or any unix shell, you can use the command "basic filename.bas"
to run a Basic program, and that externally edited Basic program
do not need to have or use line numbers.

Every personal computer should come with a simple, easy to learn,
programming language.  Chipmunk Basic was my contribution for the
very first PowerMacs.  Chipmunk Basic only comes with a man page and
a quick reference to the Mac specific functions.  The language is
mostly compatible with books on programming in BASIC that were
written between around 1978 and 1990. This version is a both bug
fix and new feature release.  It is still free for educational and
non-commercial distribution and use (but only for those who don't
believe that using the BASIC language causes brain damage. :-)

Please send bug reports to <mailto:rhn@nicholson.com>
More documentation and possible updates can be found on the
Chipmunk Basic Home Page:  <http://www.nicholson.com/rhn/basic>   

Shortened version history:

Version 3.6.6(b0): 
 	fixed a gosub error message
        fixed some graphics commands under OS X 10.7
	added mat read, fixed mat assign bug
Version 3.6.5(b3): 
        fixed mat multiply
        fixed bug in format$() with leading zeros
        fixed bug in exit while statement
        fixed bugs in empty for and empty edit statements
        fixed object string bug
Version 3.6.4(b8): 
        fixed problems with fn plot1, format$, string objects
	added command: graphics arc x,y,r,a1,a2
Version 3.6.4(b7): 
        fixed some mat command syntax omissions
        fixed a function subroutine return bug
        allow subroutines to return 1d and 2d mat arrays
        added beta test object arrays
Version 3.6.4(b6): 
	added def local
Version 3.6.4(b5): 
        added a TextWrangler AppleScript utility
        allow restore command to use a labeled line
        added fn playsound() to play sound files
        fixed sound command for some multivoiced tones
        fixed graphics pict to work with more image files
        added fn eval()
        added #ifndef _chipmunkbasic_ to ignore code
        fixed documentation on 2 parameter atan()
Version 3.6.4(b1): allow larger bload/bsave file sizes
        added det() function to calculate 2d matrix determinants
        added fn dot(a,b) to calculate 1d vector dot product
        allow mat inv of larger matrices
        allow larger bload/bsave file sizes
        allow if-then else syntax without a colon :
        allow comments at beginning of if-endif statement blocks
        improved fn sleep() timing
        fixed some bugs in format$() and print using
        fixed default save button highlight in Mac Intel build
Version 3.6.3(b1): added fn fft1(), fixed get & randomize/rnd bug
Version 3.6.3(b0): added dbm database command, fixed fn math$() bug,
        fixed macfunction "putstr2clip"
Version 3.6.2(b9): fixed del bug, graphics window bug, format$(),
        MacOS X Intel port + random file byte order fix, fn version$()
Version 3.6.2(b5): added system$(), fn version$, open pipe for output,
        fixed atn() bug, fixed Mac bundle name & icon, savepicture
Version 3.6.1(b3): fixed integer LET command bug
        added morse, say, sound & com1: support to command-line basic
        documented fseek command
Version 3.6.1: changed exponentiation precedence, default mat origin
        added mat print command
Version 3.6.0: added exit status, fn kill(), fn bigendian(),
        added Carbon graphics scrn() function.
        Included an AppleScript for use with TextEdit
Other additions:
    unix socket() and pipe i/o functions
    Carbon window: serial port i/o, sound recording,
        saved preferences for font, changed path used for "Save As"
Version 3.5.9b4: added two parameter atn()
Version 3.5.9b2: fixed "Save As", intl. string compares
Version 3.5.8b4: fixed inkey$. changed int() to round to -infinity.

 * Chipmunk Basic is Copyright 1994-2012 by Ronald H. Nicholson, Jr.
 * ALL RIGHTS RESERVED
 *
 * Permission to use, copy and distribute this software without fee
 * for non-commercial or educational purposes is hereby granted,
 * provided that the above copyright notice appear in all copies,
 * and that both the copyright notice and this permission notice with
 * the following disclaimer appear in the supporting documentation.
 *
 * This program is distributed in the hope that it will be useful, but
 * WITHOUT ANY WARRANTY OF ANY KIND; not even the implied warranty of
 * MERCHANTABILITY or FITNESS FOR ANY PARTICULAR PURPOSE.
 
 * Portions of this version of Chipmunk Basic might be
 *   Copyright (c) 1983 Regents of the University of California.
 * Portions of Chipmunk Basic might be Copyright (C) 1989 Dave Gillespie.

-- cut here --
