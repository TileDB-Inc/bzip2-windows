# bzip2-windows
Repository for bzip2 Windows builds (dependency of TileDB on Windows).

The source is unmodified from the [official sources](http://bzip.org), but we have added the required files for building with CMake.

# To build

1. Open PowerShell. Ensure the CMake bin directory is in your PATH. For example, if you have Visual Studio 2017 Community Edition installed, use the following:
```
PS> $env:Path += ";C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\Common7\IDE\CommonExtensions\Microsoft\CMake\CMake\bin"
```

2. Execute the following commands:
```
PS> cd bzip2-VERSION
PS> mkdir build
PS> cd build
PS> cmake ..
PS> cmake --build .
```

This will build both a shared and static version of the bzip2 library.
