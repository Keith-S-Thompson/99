The 99 programming language is a special-purpose language specifically
created for the [99 Bottles of Beer](http://99-bottles-of-beer.net/)
web site.

[NOTE: On Sun 2011-08-28 I retroactively changed the author
information in all checkins.  Nothing nefarious, just cleanup.
If you've pulled this repository before, please pull it again.]

99-bottles-of-beer.net is a collection of (as of Sat 2012-09-15)
1500 different programs in different languages, each if which prints
the lyrics to the song "99 Bottles of Beer on the Wall".

When I ran across this site in 2004, I realized that the existing
programs were far too verbose, with their loops, subroutines,
print statements, and so forth.

So I invented the 99 language.

The language definition is relatively straightforward.

Syntax:

- A 99 program consists of a single text file.

- On each line, everything from a `#` character to the end of the
  line is ignored, i.e., comments are introduced by `#` characters.
  (Unlike some other languages, `#` characters within character
  constants and string literals are not an issue.)

- After comments are stripped, leading and trailing white space
  are ignored.

- Empty lines are ignored.

- Anything not ignored is a syntax error.

Semantics:

- A syntactically valid 99 program, when executed, prints the lyrics
  to the song "99 Bottles of Beer on the Wall".

This distribution includes a 99 interpreter "99", written in Perl 5,
two sample 99 program, `99.99` and `empty.99`, and a sample output
file, `99.99.out`.  The interpreter can read its input either
from a file named on the command line, or from standard input if no
arguments are given.  The interpreter implements a language extension,
permitting multiple input files to be treated as a single 99 program;
this extension is not supported by the language definition, as no
actual use for it has been discovered.

For your convenience, most systems already include a sample 99 program,
typically called `/dev/null` (on Unix-like systems), `NUL:` (CP/M,
MS-DOS and Windows), `NIL:` (Amiga), `NL:`, or `NLA0:` (OpenVMS).

This project was originally hosted on my Roadrunner home page, at
http://home.san.rr.com/smov/99/, but Roadrunner decided to delete
user home pages without notifying me.

I have received a massive number[*] of requests for a compiler for
this language.  I will continue to consider such requests for the
forseeable future.

References:

- https://github.com/Keith-S-Thompson/99
- http://99-bottles-of-beer.net/language-99-804.html
- http://esolangs.org/wiki/99

[*] Yes, 1 can be a massive number if you use a big enough font.

   -- Keith Thompson <Keith.S.Thompson@gmail.com> Sat 2012-09-15
