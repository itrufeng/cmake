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

## Static library & Dynamic library

```cmake
add_library(<name> [STATIC | SHARED | MODULE]
            [EXCLUDE_FROM_ALL]
            source1 [source2 ...])
```

[Reference](https://cmake.org/cmake/help/v3.4/command/add_library.html) [Example for static](make_a_static_library) [Example for dynamic](make_a_dynamic_library)

## Multi-directory

```cmake
add_subdirectory(source_dir [binary_dir]
                 [EXCLUDE_FROM_ALL])
```

[Reference](https://cmake.org/cmake/help/v3.4/command/add_subdirectory.html) [Example](a_project)

## Install

```cmake
install(<FILES|PROGRAMS> files... DESTINATION <dir>
        [PERMISSIONS permissions...]
        [CONFIGURATIONS [Debug|Release|...]]
        [COMPONENT <component>]
        [RENAME <name>] [OPTIONAL])
```

[Reference](https://cmake.org/cmake/help/v3.4/command/install.html?highlight=install#installing-files) [Example](install_a_project)

### How to uninstall

Because cmake doesn't support uninstall, so that we should use `shell`.

```shell
xargs rm < install_manifest.txt
```

