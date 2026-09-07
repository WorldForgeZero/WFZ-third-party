# WFZ Third-Party

Prebuilt third-party dependencies used by World Forge Zero projects.

This repository contains development files required to build WFZ components
without rebuilding third-party libraries from source.

## Contents

Dependencies may include:

- Public headers
- Static libraries
- License files
- Build/source information

Source code and unnecessary runtime/build artifacts are not included.

## Platforms

Currently supported:

- Linux x86_64 (`linux_amd64`)
- Windows x86_64 with MinGW-w64 (`win64_mingw`)

## Structure

Each dependency contains an `info` file describing its version, upstream
source, and build or package information.

Platform-specific files are stored in their respective platform directories.

Example:

    library/
    ├── info
    ├── LICENSE
    ├── linux_amd64/
    │   ├── include/
    │   └── lib/
    └── win64_mingw/
        ├── include/
        └── lib/

Some header-only libraries may use a simpler structure.

## Licensing

Third-party components remain subject to their respective licenses.
See the `LICENSE` file inside each dependency directory for details.
