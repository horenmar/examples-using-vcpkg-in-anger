# What happens if you use `builtin-baseline` to specify the version baseline

Try building this project with vcpkg checked out at
`110c50d4700794d87d95138cd8c1b3bbfee9bab5` or older, to see a build
failure due to failed resolution.

**Example build invocation**
```
cmake -B build -S . -DCMAKE_TOOLCHAIN_FILE=~/vcpkg/scripts/buildsystems/vcpkg.cmake
```
