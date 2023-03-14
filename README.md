# vcpkg_easy_startup

**The** c++ package manager.

## Quick introduction to vcpkg

vcpkg is a package manager for C++ libraries on Windows, Linux, and macOS.
It provides a simple command-line interface for installing and managing C++ libraries, with features such as dependency resolution, version management, and integration with build systems like CMake.

Using vcpkg can make it easier to manage dependencies in your C++ projects, especially if you are working on multiple platforms or with many libraries.
It can help you avoid issues with library compatibility and version mismatches, as well as save time by automating the installation and management of libraries.

Additionally, vcpkg provides a large catalog of C++ libraries that you can easily search and install, which can save you the trouble of manually downloading and building each library yourself.

## Prerequisites

### General Prerequisites: 
On either Linux or Windows
- Powershell v6 + must be installed. Current versions 7.1.x are recommanded and work for both platforms.
- Git must be installed.

### Prerequisites for Windows build target (Debug or Release configuration)
- Visual Studio 2022 with C++ Desktop development module installed
- Clone [VCPKG repo](https://github.com/microsoft/vcpkg.git) in your main development directory. You put it somewhere else, just consider to update the CMakePresets variable correctly.

### Prerequisites for Linux build target (Linux-GCC-Debug or Linux-GCC-Release configuration)

.. Later on ...

## How to deploy vcpkg on your project

- Copy and past vcpkg.json and vcpkg-configuration.json files into your project repository.
- Update both file on all @todo@ sections.
- Add the needed dependancies on vcpkg.json file.
- Don't forget to update the CMAKE_TOOLCHAIN_FILE variable from your CMakePresets.json if needed.
- Ready to go !

Now you can find_package any of your library.

**NOTE:** If vcpkg is not recognize, don't forget to remove your local cache and re-generate it.

## How to create a vcpkg package

.. Later on ...