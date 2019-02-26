# xcoreutils-seq
C++ rewrite of the GNU coreutils seq utility.

# Building
Instructions for building the package.

## Windows
> TODO: Update build command to use x64 host toolchain.
```
cmake -G "Visual Studio 15 2017 Win64" -DCMAKE_TOOLCHAIN_FILE="C:/vcpkg/scripts/buildsystems/vcpkg.cmake" . --target ../xcoreutils-seq
cmake --build .
```
