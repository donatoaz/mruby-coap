# mruby-coap
[![Build Status](https://travis-ci.org/lurkshark/mruby-coap.svg?branch=master)](https://travis-ci.org/lurkshark/mruby-coap)

## Installing

This package depends on the stable version of
[libcoap](https://libcoap.net/doc/install.html). To build it:

```bash
git clone https://github.com/obgm/libcoap.git
git pull origin master
git checkout master
./autogen.sh
./configure --prefix=INSTALL_PATH --disable-examples
make
make install
```
After that, checkout this repo

```bash
git clone https://github.com/donatoaz/mruby-coap.git
```

Edit the mrbgem.rake to adjust the include and libcoap-1 path (as per the
--prefix above).

```bash
cd mruby-coap && ruby run_test.rb test
```

## Special Thanks to

[lurkshark/mruby-coap](https://github.com/lurkshark/mruby-coap) for providing the original code.
