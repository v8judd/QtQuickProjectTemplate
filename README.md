# Project template for QtQuick QML projects

This project is a template for all my future projects developed with Qt QML. It provides
a clean and scalable structure for all components of a project.  

## Directory structure overview

```
 + project root
 |  CMakeLists.txt
 |  README.md
 |  LICENSE
 |
 +-- src
 |    +-- CMakeLists.txt
 |    +-- app
 |    |    +-- CMakeLists.txt
 |    |    +-- application.h
 |    |    +-- application.cpp
 |    |    +-- main.cpp
 |    +-- core
 |    |    +-- CMakeLists.txt
 |    |    +-- backend.h
 |    |    +-- backend.cpp
 |    +-- libs
 |    |    +-- CMakeLists.txt
 |    |    +-- lib1
 |    |    |   +-- .h
 |    |    |   +-- .cpp
 |    |    +-- lib2
 |    |    |   +-- .h
 |    |    |   +-- .cpp
 |    +-- modules
 |    |   +-- CMakeLists.txt
 |    |   |   +-- module1
 |    |   |   +-- module2
 |    +-- ui
 |    |   +-- CMakeLists.txt
 |    |   +-- Main.qml
 |    |   +-- Xxx.qml
 +-- tests
 |   +-- CMakeLists.txt
 |   +-- test1
 |   |
 |   +-- test2
 |   |
```

---
### Directory details

Each directory contains a `CMakeLists.txt` file. The file in the projects root directory defines the project
and sets up the Qt CMake environment.  
* **src/app:** This directory contains all source code `*.hpp, *.cpp` files to build the single application executable for the project.
* **src/core:** Defines the C++ backend to which the QML frontend connects through the app.
* **src/libs:** Libraries developed for the project
* **src/modules:** Additional QML modules like components or custom controls.
* **src/ui:** Defines the UI for the project app.  

* **tests/...**: Contains test projects for the application.

