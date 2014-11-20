Code::Blocks Configuration for Compiler contik-cygwin-gcc

Copy working Cygwin configuration to compiler called contik-cygwin-gcc

Toolchain Executables

Installation Directory C:\Apps\Cygwin1_7

Tab: Additional Paths 
   C:\Apps\Cygwin1_7\bin

Tab: Program Files
   C Compiler: i686-pc-cygwin-gcc.exe

   Linker for dynamic Libs: i686-pc-cygwin-gcc.exe

   Linker for static Libs: ar.exe

   Make program: make.exe CC="$(TARGET_CC)" LD="$(TARGET_LD)" AR="$(TARGET_LIB)"

NOTE: Some unknown reason i686-pc-cygwin-gcc-ar.exe does NOT work to link.

Code::Blocks Project Settings
   Custom Variables
      make_os HOST_OS=Windows
      make_target TARGET=win32

   "Make" Commands
      Build Project/Target:   $make -f $makefile $(make_target) $(make_os) V=1
      Clean Project/Target:   $make -f $makefile $(make_target) $(make_os) clean
      Ask if rebuild:         $make -q -f $makefile $(make_target) $(make_os)
