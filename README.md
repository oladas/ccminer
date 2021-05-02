# ccminer

Based on Christian Buchner's &amp; Christian H.'s CUDA project, no more active on github since 2014.
Based on Tanuyg Privot's repository, cloned to compile on latest CUDA Toolkit Version

Check the [README.txt](README.txt) for the additions

BTC donation address: bc1qnp66cz7eqcs4r5209y36xmse7dms6t3qvk6yd3 (oladas)

A part of the recent algos were originally written by [djm34](https://github.com/djm34) and [alexis78](https://github.com/alexis78)

This variant was tested and built on Linux (ubuntu server 18.04)
It is also built for Windows 7 to 10 with VStudio 2013, to stay compatible with Windows 7 and Vista.

Note that the x86 releases are generally faster than x64 ones on Windows, but that tend to change with the recent drivers.

The recommended CUDA Toolkit version was the [6.5.19](http://developer.download.nvidia.com/compute/cuda/6_5/rel/installers/cuda_6.5.19_windows_general_64.exe), but some light algos could be faster with the version 7.5 and 8.0 (like lbry, decred and skein).
Compiled with Cuda Toolkit 11.3

About source code dependencies
------------------------------

This project requires some libraries to be built :

- OpenSSL (prebuilt for win)
- Curl (prebuilt for win)
- pthreads (prebuilt for win)

The tree now contains recent prebuilt openssl and curl .lib for both x86 and x64 platforms (windows).

To rebuild them, you need to clone this repository and its submodules :
    git clone https://github.com/peters/curl-for-windows.git compat/curl-for-windows


Compile on Linux
----------------

Edit Makefile.am and execute build.sh