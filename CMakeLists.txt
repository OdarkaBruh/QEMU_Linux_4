project(hello)



ADD_LIBRARY( MyStaticLib STATIC

             hello2.c )





# CMake instructions to test using the static lib



SET( APP_EXE StaticTest )



ADD_EXECUTABLE( ${APP_EXE}

                hello1.c ) 



TARGET_LINK_LIBRARIES( ${APP_EXE}

                       MyStaticLib )
