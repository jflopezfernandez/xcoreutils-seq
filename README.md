# xcoreutils-seq
C++ rewrite of the GNU coreutils seq utility.

# Building
Instructions for building the package. Both of these examples assume the build directory and the source directory are located side by side in a directory.

## Windows
Vcpkg is assumed on Windows. You must run `vcpkg integrate install` to access installed libraries. In addition, you must also configure any CMake projects to use the toolchain file, which is shown below.
```
cmake -G "Visual Studio 15 2017 Win64" -DCMAKE_TOOLCHAIN_FILE="C:/vcpkg/scripts/buildsystems/vcpkg.cmake" -Thost=x64 . --target ../xcoreutils-seq
cmake --build .
```

## Linux
I used default settings for the build, which results in using GCC 8.2.1 on Manjaro Linux. The `CMakeLists.txt` file sets the project-wide C++ language standard to C++17, so if your compiler cannot meet that requirement, you may need to tweak your settings here, which you can do as usual.
```
cmake ../xcoreutils-seq
cmake --build .
```
