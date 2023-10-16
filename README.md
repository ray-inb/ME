# surfaceCONTROL Maintenance Desktop-App and Service

## How to Build it
to build the Maintenance Desktop-app and the Service, you need the following Toolset:
- **CMake**: Install with DSM
- **Conan**: Install witg DSM. After Installation
- **[Ninja](https://github.com/ninja-build/ninja/releases)**: Unzip in some directory (e.g. C:\Ninja) and add this path to the PATH environment variable.

After installing all of them you have to download another Conan-Configuration to use Conan in CMake-Projects only when needed. Open a terminal and execute:

```
conan config install https://gitlab02.micro-epsilon.me-group.local/inb-vision/packages.git
```

**If you use Visual Studio Code**, you have to configure the CMake-Extension to use Ninja as the preferred Generator. Open **Settings** ans Search in the upper Text-Field for **CMake Generator**. In the upcoming Settings **CMake Generator**, type **Ninja** and close the Settings tab.

Now you are prepared to Build the entire Maintenance Suite. Just clone or open the Project in Visual Studio Code.

## Documentation

- [Introduction](docs/introduction.md)
- [Communication: The Device Maintenance Control Protocol](docs/dmcp.md)
