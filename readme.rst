==============
Delayed output
==============

A tiny tool that takes stdin, and output to stdout line by line with delay.

Usage: ``python delay-output.py {seconds} { { -b | -c | --per-byte | --per-char } num }``

If one of (``-b``, ``-c``, ``--per-byte``, ``-per-char``) specified, output will be delayed by ``num`` characters (bytes), not lines.

**Warning**: Delayed output means many bytes will be buffered in the pipe, I'm not sure if your kernel crashes or not.
