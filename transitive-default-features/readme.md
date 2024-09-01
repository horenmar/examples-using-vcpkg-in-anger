
Configure as with `cmake -B build-test -S . -DCMAKE_TOOLCHAIN_FILE=c:/ubuntu/vcpkg/scripts/buildsystems/vcpkg.cmake`
_Adjust your path to vcpkg as needed._

Expected output for direct use
```
c:\ubuntu\presentations\lightning-talks\vcpkg-is-a-great-tool\vcpkg-examples\transitive-default-features>cmake -B build-test -S . -DCMAKE_TOOLCHAIN_FILE=c:/ubuntu/vcpkg/scripts/buildsystems/vcpkg.cmake
-- Building for: Visual Studio 16 2019
-- Running vcpkg install
Fetching registry information from https://github.com/Microsoft/vcpkg (HEAD)...
Detecting compiler hash for triplet x64-windows...
The following packages will be built and installed:
  * libpng:x64-windows -> 1.6.39#1 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\af144fe56e6e4c08cd8089d2e1dd46bae60a5062
    opencv4[core,png]:x64-windows -> 4.8.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\0bae188d52a71f441df28b25278e5506502dfd03
  * vcpkg-cmake:x64-windows -> 2022-12-22 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\1913f86defd2140d0a6751be2d51952e4090efa4
  * vcpkg-cmake-config:x64-windows -> 2022-02-06#1 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\8d54cc4f487d51b655abec5f9c9c3f86ca83311f
  * vcpkg-get-python-packages:x64-windows -> 2022-06-30 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\e65762bfef05a4d380bb171409c48a694fb35435
  * zlib:x64-windows -> 1.2.13 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\ad5a49006f73b45b715299515f31164131b51982
```

Expected output for indirect use

**Windows**
```
Fetching registry information from https://github.com/Microsoft/vcpkg (HEAD)...
Detecting compiler hash for triplet x64-windows...
The following packages will be built and installed:
    libfoo:x64-windows -> 0.0.0 -- C:/ubuntu/presentations/lightning-talks/vcpkg-is-a-great-tool/vcpkg-examples/transitive-default-features/foosdk/overlay-ports\libfoo
  * libjpeg-turbo:x64-windows -> 2.1.5.1#1 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\2764640a1b2cc36636084470108de50f2b531085
  * liblzma:x64-windows -> 5.4.1#1 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\9a3ebbf75e1c3adb76d7e71717c1f03bb291036a
  * libpng:x64-windows -> 1.6.39#1 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\af144fe56e6e4c08cd8089d2e1dd46bae60a5062
  * libwebp[core,libwebpmux,nearlossless,simd,unicode]:x64-windows -> 1.3.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\d11b6a22e2acdba95c761dd4045cd8d66095f42d
  * opencv4[core,default-features,dnn,jpeg,png,quirc,tiff,webp]:x64-windows -> 4.8.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\0bae188d52a71f441df28b25278e5506502dfd03
  * protobuf:x64-windows -> 3.21.12 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\3b145508ba614fe26989b23f6317f15bf6467be4
  * quirc:x64-windows -> 1.1#3 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\85b17d675bbbb05448d16af79d434bc5fca51f7b
  * tiff[core,jpeg,lzma,zip]:x64-windows -> 4.5.0#3 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\658dc44e4f5495f0820db6358d8edf74e6ac8d48
  * vcpkg-cmake:x64-windows -> 2022-12-22 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\1913f86defd2140d0a6751be2d51952e4090efa4
  * vcpkg-cmake-config:x64-windows -> 2022-02-06#1 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\8d54cc4f487d51b655abec5f9c9c3f86ca83311f
  * vcpkg-get-python-packages:x64-windows -> 2022-06-30 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\e65762bfef05a4d380bb171409c48a694fb35435
  * zlib:x64-windows -> 1.2.13 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\ad5a49006f73b45b715299515f31164131b51982
```

**Linux**
```
Detecting compiler hash for triplet x64-linux...
The following packages will be built and installed:
  * at-spi2-atk:x64-linux -> 2.38.0 -- /home/xarn/.cache/vcpkg/registries/git-trees/ebb28a9cdbd06d3185ba2e0cfc1945be23a0a608
  * at-spi2-core:x64-linux -> 2.44.1#2 -- /home/xarn/.cache/vcpkg/registries/git-trees/897df7693a8a1addc3a5ab84efabef89e4cef1d8
  * atk:x64-linux -> 2.38.0#5 -- /home/xarn/.cache/vcpkg/registries/git-trees/0287be8f06bb4da8b89f9edb0aa93258c6d36f1e
  * brotli:x64-linux -> 1.0.9#5 -- /home/xarn/.cache/vcpkg/registries/git-trees/32ea6c4b0d18fa3172ad52147599983acc71d748
  * bzip2[core,tool]:x64-linux -> 1.0.8#4 -- /home/xarn/.cache/vcpkg/registries/git-trees/6165360d15e6de08dff3a5f079d51e69908cc55d
  * cairo[core,fontconfig,freetype,gobject,x11]:x64-linux -> 1.17.8 -- /home/xarn/.cache/vcpkg/registries/git-trees/062c7e11a8b910e76a2f16e57e3ffe0d59bd905e
  * dirent:x64-linux -> 1.23.2#2 -- /home/xarn/.cache/vcpkg/registries/git-trees/9d27b241631b1f540dd16824cd8a2df735233733
  * egl-registry:x64-linux -> 2022-09-20 -- /home/xarn/.cache/vcpkg/registries/git-trees/e596b6c29ad16da764aab6f2fef830a3a884f14b
  * expat:x64-linux -> 2.5.0#3 -- /home/xarn/.cache/vcpkg/registries/git-trees/9a1bc114edd74892d292c799e7b45b407f2a0b8b
  * fontconfig:x64-linux -> 2.14.2 -- /home/xarn/.cache/vcpkg/registries/git-trees/26490bc4c9aa1377da98980ba6e1089525fdaa55
  * freetype[brotli,bzip2,core,png,zlib]:x64-linux -> 2.12.1#3 -- /home/xarn/.cache/vcpkg/registries/git-trees/db92ea87ff12339808263710675221df6a06ac15
  * fribidi:x64-linux -> 1.0.12 -- /home/xarn/.cache/vcpkg/registries/git-trees/43f84b32dcc2e675fac20a42c0cf0c7f801c1fbc
  * gdk-pixbuf:x64-linux -> 2.42.10 -- /home/xarn/.cache/vcpkg/registries/git-trees/39ca957973ae4f5cbeb0e658172c079e6ad0362c
  * getopt:x64-linux -> 0#3 -- /home/xarn/.cache/vcpkg/registries/git-trees/ba541c1ce4012fae6dfdf34021b03d7253235b24
  * gettext[core,tools]:x64-linux -> 0.21.1#1 -- /home/xarn/.cache/vcpkg/registries/git-trees/6cc01d324fb1fc9a461212e5577ec9897d7da345
  * gettext-libintl:x64-linux -> 0.21.1 -- /home/xarn/.cache/vcpkg/registries/git-trees/783d7b1a2ddaf29b0f1a2d785ccfbb4a05615667
  * glib:x64-linux -> 2.76.2 -- /home/xarn/.cache/vcpkg/registries/git-trees/219fb684c85e933ff56764423c86055a7a23ee62
  * gperf:x64-linux -> 3.1#5 -- /home/xarn/.cache/vcpkg/registries/git-trees/c1dc7145f2a0607798bfdaede7bf064b88e908ac
  * gtk3:x64-linux -> 3.24.37 -- /home/xarn/.cache/vcpkg/registries/git-trees/f4e197166d448971a8856734debc428f05b456cb
  * harfbuzz:x64-linux -> 7.2.0 -- /home/xarn/.cache/vcpkg/registries/git-trees/6715cbef7e30e10a6888a737e49a3f971b08f24c
  * libepoxy:x64-linux -> 1.5.10#1 -- /home/xarn/.cache/vcpkg/registries/git-trees/76a3ae8e21ad9736741ecc58522805647fdbb7b9
  * libffi:x64-linux -> 3.4.4#1 -- /home/xarn/.cache/vcpkg/registries/git-trees/2422375e9ac93e01de0b511e1181000c340da613
    libfoo:x64-linux -> 0.0.0 -- /mnt/c/ubuntu/presentations/lightning-talks/vcpkg-is-a-great-tool/vcpkg-examples/transitive-default-features/foosdk/overlay-ports/libfoo
  * libiconv:x64-linux -> 1.17#1 -- /home/xarn/.cache/vcpkg/registries/git-trees/4226589d5d658f4d96df83f8539de54dc57a5996
  * libjpeg-turbo:x64-linux -> 2.1.5.1#1 -- /home/xarn/.cache/vcpkg/registries/git-trees/2764640a1b2cc36636084470108de50f2b531085
  * liblzma:x64-linux -> 5.4.1#1 -- /home/xarn/.cache/vcpkg/registries/git-trees/9a3ebbf75e1c3adb76d7e71717c1f03bb291036a
  * libpng:x64-linux -> 1.6.39#1 -- /home/xarn/.cache/vcpkg/registries/git-trees/af144fe56e6e4c08cd8089d2e1dd46bae60a5062
  * libuuid:x64-linux -> 1.0.3#13 -- /home/xarn/.cache/vcpkg/registries/git-trees/356948d66a6dd59bd830d26c78d1df673de20ea1
  * libwebp[core,libwebpmux,nearlossless,simd]:x64-linux -> 1.3.0 -- /home/xarn/.cache/vcpkg/registries/git-trees/d11b6a22e2acdba95c761dd4045cd8d66095f42d
  * libxml2[core,iconv,lzma,zlib]:x64-linux -> 2.10.3#1 -- /home/xarn/.cache/vcpkg/registries/git-trees/fd1e750ce7851d72bf39c0b6d30a4a8d1d717c45
  * lzo:x64-linux -> 2.10#9 -- /home/xarn/.cache/vcpkg/registries/git-trees/fcd8844a4e80d418bf894cf93a0453f067e404de
  * opencv4[core,default-features,dnn,gtk,jpeg,png,quirc,tiff,webp]:x64-linux -> 4.8.0 -- /home/xarn/.cache/vcpkg/registries/git-trees/0bae188d52a71f441df28b25278e5506502dfd03
  * pango:x64-linux -> 1.50.14 -- /home/xarn/.cache/vcpkg/registries/git-trees/3985e71b9e3446f57995321a290a75a7bf5101dc
  * pcre2[core,jit,platform-default-features]:x64-linux -> 10.40#2 -- /home/xarn/.cache/vcpkg/registries/git-trees/533fc8ada3da33f695eb499fe8190a5e9b24a5c8
  * pixman:x64-linux -> 0.42.2#2 -- /home/xarn/.cache/vcpkg/registries/git-trees/a51c895edc5dd8067f51b600d631a5e8b32a65e8
  * protobuf:x64-linux -> 3.21.12 -- /home/xarn/.cache/vcpkg/registries/git-trees/3b145508ba614fe26989b23f6317f15bf6467be4
  * pthread:x64-linux -> 3.0.0#2 -- /home/xarn/.cache/vcpkg/registries/git-trees/e32a8cb12153277234e7c7e04322bdf90580659a
  * pthreads:x64-linux -> 3.0.0#14 -- /home/xarn/.cache/vcpkg/registries/git-trees/2e0a6df2800d3677b941dc6504f083965b7886d9
  * quirc:x64-linux -> 1.1#3 -- /home/xarn/.cache/vcpkg/registries/git-trees/85b17d675bbbb05448d16af79d434bc5fca51f7b
  * tiff[core,jpeg,lzma,zip]:x64-linux -> 4.5.0#3 -- /home/xarn/.cache/vcpkg/registries/git-trees/658dc44e4f5495f0820db6358d8edf74e6ac8d48
  * vcpkg-cmake:x64-linux -> 2022-12-22 -- /home/xarn/.cache/vcpkg/registries/git-trees/1913f86defd2140d0a6751be2d51952e4090efa4
  * vcpkg-cmake-config:x64-linux -> 2022-02-06#1 -- /home/xarn/.cache/vcpkg/registries/git-trees/8d54cc4f487d51b655abec5f9c9c3f86ca83311f
  * vcpkg-get-python-packages:x64-linux -> 2022-06-30 -- /home/xarn/.cache/vcpkg/registries/git-trees/e65762bfef05a4d380bb171409c48a694fb35435
  * vcpkg-tool-meson:x64-linux -> 0.63 -- /home/xarn/.cache/vcpkg/registries/git-trees/bee0cb6c5edf45133ebc9643b86c9c775ab36cfe
  * zlib:x64-linux -> 1.2.13 -- /home/xarn/.cache/vcpkg/registries/git-trees/ad5a49006f73b45b715299515f31164131b51982
Additional packages (*) will be modified to complete this operation.
Restored 0 package(s) from /home/xarn/.cache/vcpkg/archives in 34.5 ms. Use --debug to see more details.
Installing 1/45 vcpkg-cmake-config:x64-linux...
```
