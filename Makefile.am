EXTRA_DIST = GameWorld.h GameAssetManager.h GameAsset.h CubeAsset.h Boundingbox.h Math.h 
 
bin_PROGRAMS = shaderexample
shaderexample_SOURCES = main.cc GameWorld.cc GameAssetManager.cc CubeAsset.cc Boundingbox.cc 

AM_CPPFLAGS = -DGL_GLEXT_PROTOTYPES -DGL3_PROTOTYPES
AM_CPPFLAGS += -std=c++11
AM_CPPFLAGS += $(gl_CFLAGS) $(glew_CFLAGS) $(sdl2_CFLAGS) $(BOOST_CPPFLAGS)
LIBS += $(gl_LIBS) $(glew_LIBS) $(sdl2_LIBS) $(BOOST_THREAD_LIBS) $(BOOST_PROGRAM_OPTIONS_LIBS)

TESTS = TESTTRY
check_PROGRAMS = $(TESTS)
TESTTRY_SOURCES = Testboundingbox.cpp
TESTTRY_LDADD = $(BOOST_UNIT_TEST_FRAMEWORK_LIBS)
