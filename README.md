LZ4 - dll: Visual Studio Project
================================
Visual Studio project to create LZ4 dlls.

This repo contains a Visual Studio 2013 project to create dlls from the LZ4 library.
The dlls are relative only to the core functions of LZ4 and LZ4HC.

# Compiling
The version of LZ4 synchronized with this repo is the **r131**.
Because the branch master of LZ4 is always stable, you can always update the LZ4 submodule to the most recent version on the branch master.

# Using the dlls
The dlls export the following functions of LZ4:

For the same functions are provided also entry points. To keep it simple the entry point have similar names of the function, the only difference is that the prefix of the library functions is "LZ4_" while the prefix of the entry points is "Lz4_".

# About LZ4
LZ4 is lossless compression algorithm, 
providing compression speed at 400 MB/s per core, 
scalable with multi-cores CPU. 
It also features an extremely fast decoder, 
with speed in multiple GB/s per core, 
typically reaching RAM speed limits on multi-core systems.

Speed can be tuned dynamically, selecting an "acceleration" factor
which trades compression ratio for more speed up.
On the other end, a high compression derivative, LZ4_HC, is also provided,
trading CPU time for improved compression ratio.
All versions feature the same excellent decompression speed.

The LZ4 library is released under the BSD - 2 license.
For other details please refer to the authors: https://github.com/Cyan4973/lz4 
