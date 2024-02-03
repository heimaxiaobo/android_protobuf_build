# Google protobuf-lite for Android NDK

This repository builds a static protobuf-lite library for Android.
Based on protobuf-3.12.4 as used in Ubuntu 22.04.

## Update protobuf

- Download the required [protobuf](https://github.com/protocolbuffers/protobuf/releases) version.
- Copy the `protobuf-x.x.x/src/google` folder to `jni/src`.
- Open `jni/Android.mk` and update list of files to build
  according to `protobuf-x.x.x/cmake/libprotobuf-lite.cmake`.
- Open `build.sh` and update list of include files according to
  `protobuf-x.x.x/cmake/extract_includes.bat.in`.

## Build

```shell
./build.sh
```
