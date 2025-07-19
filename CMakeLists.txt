cmake_minimum_required(VERSION 3.16)

project(QtQuickProjectTemplate VERSION 0.1 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(QT_QML_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/qml)
set(QML_IMPORT_PATH ${QT_QML_OUTPUT_DIRECTORY} CACHE PATH "Extra QML import paths to make Qt Creator happy")

find_package(Qt6 REQUIRED COMPONENTS Quick)

qt_standard_project_setup(REQUIRES 6.5)

add_subdirectory(src)
add_subdirectory(tests)


# qt_add_executable(appQtQuickProjectTemplate
#     main.cpp
# )

# qt_add_qml_module(appQtQuickProjectTemplate
#     URI QtQuickProjectTemplate
#     VERSION 1.0
#     QML_FILES
#         Main.qml
# )

# Qt for iOS sets MACOSX_BUNDLE_GUI_IDENTIFIER automatically since Qt 6.1.
# If you are developing for iOS or macOS you should consider setting an
# explicit, fixed bundle identifier manually though.
# set_target_properties(appQtQuickProjectTemplate PROPERTIES
# #    MACOSX_BUNDLE_GUI_IDENTIFIER com.example.appQtQuickProjectTemplate
#     MACOSX_BUNDLE_BUNDLE_VERSION ${PROJECT_VERSION}
#     MACOSX_BUNDLE_SHORT_VERSION_STRING ${PROJECT_VERSION_MAJOR}.${PROJECT_VERSION_MINOR}
#     MACOSX_BUNDLE TRUE
#     WIN32_EXECUTABLE TRUE
# )


# include(GNUInstallDirs)
# install(TARGETS appQtQuickProjectTemplate
#     BUNDLE DESTINATION .
#     LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
#     RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
# )
