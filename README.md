# Compress Utilities for ReactOS #

This library is designed to be compiled with the [ReactOS](http://reactos.org/) build environment. This project is maintained to help keep the program in sync whenever the original utility decides to release another version. These programs can be compiled in other compilers, but some modifications may be needed in order to build properly since some of the changes here are ReactOS specific. Enjoy!

## Original Readme ##

*mscompress*, Microsoft "compress.exe/expand.exe" compatible (de)compressor
Copyright (c) 2000 Martin Hinner <mhi@penguin.cz>
Algorithm & data structures by M. Winterhoff <100326.2776@compuserve.com>
[ftp://ftp.penguin.cz/pub/users/mhi/mscompress/](ftp://ftp.penguin.cz/pub/users/mhi/mscompress/)

This package contains two programs:

- *msexpand*, which decompress files compressed by Microsoft compress.exe utility (e.g. Win 3.x installation files)
- &mscompress*, which compress files using LZ77 compression algorithm. Output files can be decompressed using Microsoft expand.exe or msexpand(1).

To install it on your Unix box, configure the package ("./configure") and then type "make all test install".

-- mhi
