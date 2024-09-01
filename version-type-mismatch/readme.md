


Expected output for libfoo

```
c:\ubuntu\presentations\lightning-talks\vcpkg-is-a-great-tool\vcpkg-examples\version-type-mismatch\libfoo>cmake -B build-test -S . -DCMAKE_TOOLCHAIN_FILE=c:/ubuntu/vcpkg/scripts/buildsystems/vcpkg.cmake
-- Building for: Visual Studio 16 2019
-- Running vcpkg install
Fetching registry information from https://github.com/Microsoft/vcpkg (HEAD)...
Detecting compiler hash for triplet x64-windows...
The following packages will be built and installed:
    abseil:x64-windows -> 20211102.1 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\962a81319706d17c9e90bd0b873659ec7c75178a
  * vcpkg-cmake:x64-windows -> 2022-06-07 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\819e45a14fb875ec7e8373143c994b7bd8d8f7cb
  * vcpkg-cmake-config:x64-windows -> 2022-02-06#1 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\8d54cc4f487d51b655abec5f9c9c3f86ca83311f
Additional packages (*) will be modified to complete this operation.
Restored 1 package(s) from C:\Users\Xarn\AppData\Local\vcpkg\archives in 37.3 ms. Use --debug to see more details.
Installing 1/3 vcpkg-cmake-config:x64-windows...
```


Expected output for foosdk

```
version-type-mismatch\foosdk>cmake -B build-test -S . -DCMAKE_TOOLCHAIN_FILE=c:/ubuntu/vcpkg/scripts/buildsystems/vcpkg.cmake
-- Running vcpkg install
Fetching registry information from https://github.com/Microsoft/vcpkg (HEAD)...
error: version conflict on abseil:x64-windows: foosdk required 20230802.1, which cannot be compared with the baseline version 20211102.1.

The versions have incomparable schemes:
  abseil@20211102.1 has scheme string
  abseil@20230802.1 has scheme relaxed

This can be resolved by adding an explicit override to the preferred version. For example:

  "overrides": [
    { "name": "abseil", "version": "20211102.1" }
  ]

See `vcpkg help versioning` or https://learn.microsoft.com/vcpkg/users/versioning for more information.
-- Running vcpkg install - failed
CMake Error at C:/ubuntu/vcpkg/scripts/buildsystems/vcpkg.cmake:899 (message):
  vcpkg install failed.  See logs for more information:
  C:\ubuntu\presentations\lightning-talks\vcpkg-is-a-great-tool\vcpkg-examples\version-type-mismatch\foosdk\build-test\vcpkg-manifest-install.log
Call Stack (most recent call first):
  C:/Program Files/CMake/share/cmake-3.27/Modules/CMakeDetermineSystem.cmake:148 (include)
  CMakeLists.txt:4 (project)


-- Configuring incomplete, errors occurred!
```
