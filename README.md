   __  __ ___   ___ ___ 
   \ \/ /  _ \ / __/ __|
    )  (| |_) | (_| (__ 
   /_/\_\  __/ \___\___|
        | |   
        |_|  Cross Platform Component Communication
             http://roboterclubaachen.github.com/xpcc/

The xpcc project consists of two main parts:

 * First part is the xpcc communication module, a packet oriented
   communication protocol, enabling transparent communication between
   components on different platforms (from PCs to small 8-bit
   microcontrollers). It provides an interface to communicate via CAN,
   TCP/IP or TIPC.
 * The second part is a universal but a bit robotic oriented C++ library
   for microcontrollers.

The primary aim has been the usage of this system in autonomous robots for
the EUROBOT competition, but it can be used for many other purposes as well.


Get the Code
-------------------------------------------------------------------------------

$ git clone git://github.com/roboterclubaachen/xpcc.git xpcc
$ cd xpcc
$ git submodule init
$ git submodule update


Documentation
-------------------------------------------------------------------------------

The main documentation is created from doxygen files in the doc-folder. It can
be found online at http://roboterclubaachen.github.com/xpcc/api/.


Folder structure
-------------------------------------------------------------------------------

build
   Temporary folder, build files created during building the unit tests etc.
   go in here. Can be deleted to save disk space.

doc
   Documentation, mainly the doxygen documentation. The online documentation
   on http://roboterclubaachen.github.com/xpcc/api/ is build by running 'doxygen doxyfile'
   in this folder.

examples
   Example projects that show the usage of parts of the xpcc library. These
   projects are always up to date and are tested to compile before a
   release.

release
   Among other things some test programs which are run before a release to 
   check that everything is compiling correctly.

scons
   SCons tools (e.g. xpcc.py for the build process, avr.py for compiling for
   AVR microcontrollers, arm.py for compiling for ARM7 and Cortex-M0/3, etc.)
   
   Look at the SConstruct files in the example folder and the online
   documentation to see how to use the provided scons tools.

src
   Source files for the xpcc library

templates
   Template files for xpcc, Unit-Tests etc.

tests
   Test programs, used during the development of the library. May be
   out of date or not working at all.

tools
   Supporting tools for the usage of the library.

   For example the communication builder, used to generate header files for the
   communication architecture from XML-files.


How can I contribute?
-------------------------------------------------------------------------------

Use the library and give us some feedback. That's the easiest way for you and
the best way for us to see if something is unclear or missing.

If you need a specific feature just drop us a mail and we will look into it.
But don't expect a quick response, we are always busy building robots ;-)

If you want to change the library be sure to read the developer section, to
familiarize yourself with the coding convention, design decisions etc. The
source code is freely available, so feel free to adapt it to your needs. The only
thing we ask you to do is to contribute your changes back. That way everybody
can profit from it.

Have fun!
