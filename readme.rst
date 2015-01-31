==============
Delayed output
==============

A tiny tool that takes stdin, and output to stdout line by line with delay.

Usage: ``python delay-output.py {seconds} { -b | -c | --per-byte | --per-char }``

If one of (``-b``, ``-c``, ``--per-byte``, ``-per-char``) specified, output will be delayed by characters (bytes), not lines.

**Warning**: Delayed output means something will be buffered, I'm not sure what would happen when many many data are in buffer.
