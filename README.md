# Google protobuf-lite for Android NDK

This builds a static library to use protobuf-lite with C++ on Android.
Based on protobuf-3.6.1 as used in Ubuntu 20.04.

## Update protobuf

- Download the required [protobuf version](https://github.com/protocolbuffers/protobuf/releases).
- Copy the `protobuf-x.x.x/src/google` folder to `jni/src`.
- Open `jni/Android.mk` and update list of files to build
  according to `protobuf-x.x.x/cmake/libprotobuf-lite.cmake`.
- Open `build.sh` and update list of include files according to
  `protobuf-x.x.x/cmake/extract_includes.bat.in`.

## Build

```shell
./build.sh
```
