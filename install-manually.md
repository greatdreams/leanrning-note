### Steps of installing Erlang/OTP 19 from Source Code

* OS : Deepin 15.2 Desktop

#### Required Utilities


##### Unpacking

* GNU unzip, or a modern uncompress.
* A TAR program that understands the GNU TAR format for long filenames.


##### Building

* GNU make
  
  Compiler -- GNU C Compiler, gcc or the C compiler frontend for LLVM, clang.
* Perl 5
* GNU m4 -- If HiPE (native code) support is enabled. HiPE can be disabled using --disable-hipe
ncurses, termcap, or termlib -- The development headers and libraries are needed, often known as ncurses-devel. Use --without-termcap to build without any of these libraries. Note that in this case only the old shell (without any line editing) can be used.
* sed -- Stream Editor for basic text transformation.

#### Optional Utilities

Some applications are automatically skipped if the dependencies aren't met. Here is a list of utilities needed for those applications. You will also find the utilities needed for building the documentation.


#### Steps

1.Download source code of erlang/otp 19
[https://github.com/erlang/otp/releases](https://github.com/erlang/otp/releases)

2.