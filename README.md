# xcoreutils-seq
C++ rewrite of the GNU coreutils seq utility.

# Building
Instructions for building the package.

## Windows
```
cmake -G "Visual Studio 15 2017 Win64" -DCMAKE_TOOLCHAIN_FILE="C:/vcpkg/scripts/buildsystems/vcpkg.cmake" --build . --target ../xcoreutils-seq
cmake --build .
```
