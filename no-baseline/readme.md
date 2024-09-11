# What happens if you don't specify any baseline.

Try building this project with vcpkg checked out at
`c9e2aa851e987698519f58518aa16564af3a85ab` or
`fe1cde61e971d53c9687cf9a46308f8f55da19fa` to see fmt resolved at different
versions. It would be shame if the major version difference broke something.

**Example build invocation**
```
cmake -B build -S . -DCMAKE_TOOLCHAIN_FILE=~/vcpkg/scripts/buildsystems/vcpkg.cmake
```
