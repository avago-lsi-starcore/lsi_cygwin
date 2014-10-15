lsi_cygwin
==========

StarCore DSP IDE Tools modified under the GPL or the LGPL

Build HOWTO:

Extract source code:
    tar xzf lsi_cygwin.tar.gz
This will extract a "lsi_cygwin" directory.

Prepare build directory:
    mkdir build
    cd build

Build debug version:
    mkdir lsi_cygwin
    cd lsi_cygwin
    ../../lsi_cygwin/buildCygwin.sh
    cd ..

Build release version:
    mkdir lsi_cygwin-O3
    cd lsi_cygwin-O3
    ../../lsi_cygwin/buildCygwin.sh
    cd ..

Note:
The optimization level is extracted by the build script from the directory name (in this example -O3)

Summary, the directory structure should look like:
Downward from YOUR_SOURCE_DIRECTOY:
    source code:
      lsi_cygwin/etc/
      lsi_cygwin/include/
      lsi_cygwin/libiberty/
      lsi_cygwin/newlib/
      lsi_cygwin/winsup/
      lsi_cygwin/...
    debug build:
      build/lsi_cygwin/Makefile
      build/lsi_cygwin/etc/
      build/lsi_cygwin/i686-pc-cygwin/
      build/lsi_cygwin/i686-pc-cygwin/winsup/cygwin/new-lsi_cygwin1.dll
      build/lsi_cygwin/libiberty/
      build/lsi_cygwin/...
    release build:
      build/lsi_cygwin-O3/Makefile
      build/lsi_cygwin-O3/etc/
      build/lsi_cygwin-O3/i686-pc-cygwin/
      build/lsi_cygwin-O3/i686-pc-cygwin/winsup/cygwin/new-lsi_cygwin1.dll
      build/lsi_cygwin-O3/libiberty/
      build/lsi_cygwin-O3/...

