qt_add_qml_module(ui STATIC
    URI ui
    # OUTPUT_DIRECTORY "uiModule"
    RESOURCE_PREFIX "/qt/qml"
    VERSION 1.0
    QML_FILES
        Main.qml
)
