AM_CPPFLAGS = -I../.. $(CPPUNIT_CFLAGS)
AM_CXXFLAGS += $(CPPUNIT_CFLAGS)
LDADD = ../../tsk/libtsk.la $(CPPUNIT_LIBS)
LDFLAGS = -static

check_PROGRAMS = test_img
test_img_SOURCES= ../runner.cpp mult_files_test.cpp ../../tsk/img/mult_files.cpp

TESTS = $(check_PROGRAMS)

indent:
	indent *.cpp *.h

clean-local:
	-rm -f *.cpp~ *.h~
