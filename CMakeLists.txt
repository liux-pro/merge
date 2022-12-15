idf_component_register()
add_custom_target(
        merge
        COMMAND ${ESPTOOLPY} merge_bin -o ${chip_model}.bin @flash_args
        WORKING_DIRECTORY ${CMAKE_BINARY_DIR}
        DEPENDS gen_project_binary bootloader
        USES_TERMINAL
        VERBATIM
        )