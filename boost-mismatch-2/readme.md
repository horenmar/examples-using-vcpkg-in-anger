
Configure as with `cmake -B build-test -S . -DCMAKE_TOOLCHAIN_FILE=c:/ubuntu/vcpkg/scripts/buildsystems/vcpkg.cmake`
_Adjust your path to vcpkg as needed._

Expected output

```
vcpkg-examples\boost-mismatch-2>cmake -B build-test -S . ^
More?             -DCMAKE_TOOLCHAIN_FILE=c:/ubuntu/vcpkg/scripts/buildsystems/vcpkg.cmake
-- Building for: Visual Studio 16 2019
-- Running vcpkg install
Detecting compiler hash for triplet x64-windows...
The following packages will be built and installed:
  * boost-algorithm:x64-windows -> 1.82.0 -- C:\ubuntu\vcpkg\buildtrees\versioning_\versions\boost-algorithm\437bf58b244741d6ca3857cccf1b3cc937be2e4b
  * boost-array:x64-windows -> 1.82.0 -- C:\ubuntu\vcpkg\buildtrees\versioning_\versions\boost-array\b26e79e8c3b69fb7111fe82632be1cca86440b65
  * boost-assert:x64-windows -> 1.82.0 -- C:\ubuntu\vcpkg\buildtrees\versioning_\versions\boost-assert\fb48cd65e86476285b8968bf3d74c949b5c0f8bd
  * boost-bind:x64-windows -> 1.82.0 -- C:\ubuntu\vcpkg\buildtrees\versioning_\versions\boost-bind\97f32a43b457e26b8ee223c6c7201c995541d149
  * boost-build:x64-windows -> 1.82.0 -- C:\ubuntu\vcpkg\buildtrees\versioning_\versions\boost-build\cf70df3193d092c65a4b3728a5410f59e9de1c9d
    boost-circular-buffer:x64-windows -> 1.81.0 -- C:\ubuntu\vcpkg\buildtrees\versioning_\versions\boost-circular-buffer\ab5e7d9a47aa011e6fbad65cdeb6cf7d2c27c02a
```
