add_test(
    NAME TestPxrUsdTranslators
    WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}
    COMMAND
        testPxrTranslators.sh
        ${CMAKE_INSTALL_PREFIX}
        $<TARGET_FILE_DIR:plug>
        ${CMAKE_CURRENT_SOURCE_DIR}
        ${USD_MAYA_ROOT}
    )
