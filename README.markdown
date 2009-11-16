FlashZlib - Quick Guide
=======================
Port created by Ed McManus

**Follow me on Twitter!**
[http://www.twitter.com/emcmanus](http://www.twitter.com/emcmanus)


## License ##

This project is released under the zLib license. [http://www.zlib.net/zlib_license.html](http://www.zlib.net/zlib_license.html)


## Important Locations ##

  - `/bin` Contains the LLVM bitcode library to link against. This should be all you need!


## How To ##

#### Build ####

With `alc-on`, run `CFLAGS="-emit-llvm" ./configure`.

Then build and move the library with `make all; mv -f z.l.bc bin/z.l.bc`


#### Install ####

Copy `bin/z.l.bc` to your Alchemy library folder with `cp bin/z.l.bc $ALCHEMY_HOME/usr/local/lib/`, or add `./bin` to your Alchemy library path.

Copy all header files to your Alchemy include folder with `cp ./*.h $ALCHEMY_HOME/usr/local/include/`, or add this folder `./` to your Alchemy include path.