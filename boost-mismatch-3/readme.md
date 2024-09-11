
TODO!! update this



# Boost version mismatch: fix with registry slice

Configure as with `cmake -B build-test -S . -DCMAKE_TOOLCHAIN_FILE=c:/ubuntu/vcpkg/scripts/buildsystems/vcpkg.cmake`
_Adjust your path to vcpkg as needed._

Expected output

```
c:\ubuntu\presentations\lightning-talks\vcpkg-is-a-great-tool\vcpkg-examples\boost-mismatch>cmake -B build-test -S . -DCMAKE_TOOLCHAIN_FILE=c:/ubuntu/vcpkg/scripts/buildsystems/vcpkg.cmake
-- Running vcpkg install
Fetching registry information from https://github.com/Microsoft/vcpkg (HEAD)...
Detecting compiler hash for triplet x64-windows...
The following packages will be built and installed:
  * boost-assert:x64-windows -> 1.79.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\2e4adae40df44f3927978bba397b60f18ad8e919
    boost-circular-buffer:x64-windows -> 1.80.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\bf70dc530094e3190c4d5cc945bb452807cc150b
  * boost-concept-check:x64-windows -> 1.79.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\493a1b5ae991a9c7b2643e649329de16bcd0fa48
  * boost-config:x64-windows -> 1.79.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\22c6532dcc9c24fd85febb93dc936e68c031043a
  * boost-core:x64-windows -> 1.79.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\a22eddd8a3121063f8ef94eb4e0ae64021d0369a
  * boost-move:x64-windows -> 1.79.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\957381b3c5ac7d2b563b2563ca8a78d49f034e68
  * boost-predef:x64-windows -> 1.79.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\c17a7256c1f86eab749e10b451dbf53d317afaf9
  * boost-preprocessor:x64-windows -> 1.79.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\1790581b89b5cf96bd870854b2bc4b256032a9c9
  * boost-static-assert:x64-windows -> 1.79.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\673cf82169b2b1696d993477d47b2f94d4350a7f
  * boost-throw-exception:x64-windows -> 1.79.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\1607edf60f1243503820e06b4d3e16c385aa691d
  * boost-type-traits:x64-windows -> 1.79.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\7969a397a6c03205ec1c118834272183ff4201c7
  * boost-uninstall:x64-windows -> 1.79.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\e2d05f10364104d9b7de2383bcb105a1fd3fe975
  * boost-vcpkg-helpers:x64-windows -> 1.79.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\0e96a2cb3400bcafd55070d18bdcab64808ada01
  * boost-winapi:x64-windows -> 1.79.0 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\7f82a0041bb3b4ac1f3721afe5ba4e24e27c3a3c
```
