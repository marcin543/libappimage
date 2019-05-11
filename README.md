# libappimage

This library is part of the [AppImage](https://github.com/AppImage/appimagekit/) project. It implements functionality for dealing with AppImage files. It is written in C++ and is using Boost.

# How to use

As a user, you normally do not need to deal with this library. Tools that use it (like [the optional `appimaged` daemon](https://github.com/AppImage/appimaged)) usually come with a bundled copy of it.

## How to build

If for some reason you need to do a local development build, on a deb-based system (tested on Ubuntu xenial) do:

```
sudo apt-get -y install automake cmake libtool libcairo-dev libfuse-dev git
git clone https://github.com/AppImage/libappimage
cd ./libappimage/
mkdir build
cmake .. -DBUILD_TESTING:bool=False
make
sudo make install
cd ..
```
