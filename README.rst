==============
Delayed output
==============

A tiny tool that takes stdin, and output to stdout line by line with delay.

Examples
--------

* Output each line with delay 0.1 seconds

..  code :: shell

    $ ls -al | dcat -d 0.1

* Output each byte with delay 0.01 seconds

..  code :: shell

    $ ls -al | dcat -d 0.01 -c 1

* Output from file

..  code :: shell

    $ dcat -d 0.01 test-file

**Warning**: Delayed output means many bytes will be buffered in the pipe, I'm not sure what would happen if the buffer fulled.
