
find_package(Qt6 REQUIRED COMPONENTS Core)

qt_add_executable(app
    main.cpp
    application.h
    application.cpp
)

target_link_libraries(app
    PRIVATE Qt6::Quick
    uiplugin
    #backend
)
target_link_libraries(app PRIVATE Qt6::Core)
