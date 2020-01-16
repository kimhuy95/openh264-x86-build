# Build x86 binary for openh264 v2.0.0:

OpenH264 v2.0.0 source code: https://github.com/cisco/openh264/releases/download/v2.0.0/Source.Code.zip

NDK r17c (linux): https://dl.google.com/android/repository/android-ndk-r17c-linux-x86_64.zip

### x86:
`make OS=android NDKROOT='path/to/ndk/root/version-r17c' ARCH=x86 ENABLEPIC=Yes TARGET=android-28 NDKLEVEL=16`

### x86-64:
`make OS=android NDKROOT='path/to/ndk/root/version-r17c' ARCH=x86_64 ENABLEPIC=Yes TARGET=android-28 NDKLEVEL=21`

We can encounter this error when building: `build/platform-android.mk:99: recipe for target 'decdemo' failed`. This can be ignored. `libopenh264.so` binary is located in the root directory
