cmake_minimum_required(VERSION 2.6)
set(TARGET PentaZen)
project(${TARGET})

add_executable(${TARGET}
    bitboard.h
    board.c
    board.h
    display.c
    display.h
    distance.c
    distance.h
    index.h
    main.c
    mvlist.c
    mvlist.h
    pattab.c
    pattab.h
    pattern.h
    protocol.c
    protocol.h
    public.h
    search.c
    search.h
    test.c
    test.h
)

target_link_libraries(${TARGET})

if (${CMAKE_SYSTEM_NAME} MATCHES "Windows")
    set_target_properties(${TARGET} PROPERTIES LINK_FLAGS_DEBUG "/SUBSYSTEM:CONSOLE")
    set_target_properties(${TARGET} PROPERTIES LINK_FLAGS_RELWITHDEBINFO "/SUBSYSTEM:CONSOLE")
    set_target_properties(${TARGET} PROPERTIES LINK_FLAGS_RELEASE "/SUBSYSTEM:CONSOLE")
    set_target_properties(${TARGET} PROPERTIES LINK_FLAGS_MINSIZEREL "/SUBSYSTEM:CONSOLE")
endif()
