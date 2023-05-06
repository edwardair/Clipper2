
set(CLIPPER2_LIB_NAME clipper2)

aux_source_directory(src SRCS)
aux_source_directory(include HDRS)
add_library(${CLIPPER2_LIB_NAME} STATIC ${SRCS} ${HDRS})

target_include_directories(${CLIPPER2_LIB_NAME}
        PUBLIC include
        )
