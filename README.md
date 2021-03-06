# ccminer

Modified to add support for X16R (Ravencoin). Work in progress... lots of room for improvement. Use `-a x16r` and `--num-fallback-threads n` where n is > 0.

[Windows x64 builds](https://github.com/todd1251/ccminer-x16r/releases)

[Ubuntu 16.08 build instructions](https://github.com/todd1251/ccminer-x16r/wiki/Ubuntu-16.08-build)

BTC donation address: 1AJdfCpLWPNoAMDfHF1wD5y8VgKSSTHxPo (tpruvot)

RVN donation address: RWoyvvT5exmbs937QfRavf4fxB5mvijG6R (penfold)

RVN donation address: RE9hcu1LjVbzL1wzsnpnJP28B2x2Y4qc55 (phabit)

---

Based on Christian Buchner's &amp; Christian H.'s CUDA project, no more active on github since 2014.

Check the [README.txt](README.txt) for the additions

BTC donation address: 1AJdfCpLWPNoAMDfHF1wD5y8VgKSSTHxPo (tpruvot)

A part of the recent algos were originally written by [djm34](https://github.com/djm34) and [alexis78](https://github.com/alexis78)

This variant was tested and built on Linux (ubuntu server 14.04, 16.04, Fedora 22 to 25)
It is also built for Windows 7 to 10 with VStudio 2013, to stay compatible with Windows 7 and Vista.

Note that the x86 releases are generally faster than x64 ones on Windows, but that tend to change with the recent drivers.

The recommended CUDA Toolkit version was the [6.5.19](http://developer.download.nvidia.com/compute/cuda/6_5/rel/installers/cuda_6.5.19_windows_general_64.exe), but some light algos could be faster with the version 7.5 and 8.0 (like lbry, decred and skein).

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

Please see [INSTALL](https://github.com/tpruvot/ccminer/blob/linux/INSTALL) file or [project Wiki](https://github.com/tpruvot/ccminer/wiki/Compatibility)
