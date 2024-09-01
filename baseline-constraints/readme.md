

Expected output

```
vcpkg-examples\baseline-constraints>cmake -B build-test-2 -S . -DCMAKE_TOOLCHAIN_FILE=c:/ubuntu/vcpkg/scripts/buildsystems/vcpkg.cmake
-- Building for: Visual Studio 16 2019
-- Running vcpkg install
Fetching registry information from https://github.com/Microsoft/vcpkg (HEAD)...
Detecting compiler hash for triplet x64-windows...
The following packages will be built and installed:
    fmt:x64-windows -> 10.1.1 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\dfe9aa860f5a8317f341a21d317be1cf44e89f18
  * vcpkg-cmake:x64-windows -> 2023-05-04 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\88a7058fc7fa73a9c4c99cfcae9d79e2abf87a5a
  * vcpkg-cmake-config:x64-windows -> 2022-02-06#1 -- C:\Users\Xarn\AppData\Local\vcpkg\registries\git-trees\8d54cc4f487d51b655abec5f9c9c3f86ca83311f
Additional packages (*) will be modified to complete this operation.
Restored 3 package(s) from C:\Users\Xarn\AppData\Local\vcpkg\archives in 88.3 ms. Use --debug to see more details.
Installing 1/3 vcpkg-cmake-config:x64-windows...
```
