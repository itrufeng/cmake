# Hello cmake

## Version

This doc base on cmake 3.x.x

## Executable

```cmake
add_executable(<name> [WIN32] [MACOSX_BUNDLE]
               [EXCLUDE_FROM_ALL]
               source1 [source2 ...])
```

[Reference](https://cmake.org/cmake/help/v3.3/command/add_executable.html) [Example](hellocmake)

## Static library

```cmake
add_library(<name> [STATIC | SHARED | MODULE]
            [EXCLUDE_FROM_ALL]
            source1 [source2 ...])
```

[Reference](https://cmake.org/cmake/help/v3.4/command/add_library.html) [Example](make_a_static_library)

