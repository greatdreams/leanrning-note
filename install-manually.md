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

##### Building

*  OpenSSL -- The opensource toolkit for Secure Socket Layer and Transport Layer Security. Required for building the application crypto. Further, ssl and ssh require a working crypto application and will also be skipped if OpenSSL is missing. The public_key application is available without crypto, but the functionality will be very limited.

  The development package of OpenSSL including the header files are needed as well as the binary command program openssl. At least version 0.9.8 of OpenSSL is required. Read more and download from http://www.openssl.org.

Oracle Java SE JDK -- The Java Development Kit (Standard Edition). Required for building the application jinterface and parts of ic and orber. At least version 1.6.0 of the JDK is required.

Download from http://www.oracle.com/technetwork/java/javase/downloads. We have also tested with IBM's JDK 1.6.0.

X Windows -- Development headers and libraries are needed to build the Erlang/OTP application gs on Unix/Linux.

flex -- Headers and libraries are needed to build the flex scanner for the megaco application on Unix/Linux.

wxWidgets -- Toolkit for GUI applications. Required for building the wx application. At least version 3.0 of wxWidgets is required.

Download from http://sourceforge.net/projects/wxwindows/files/3.0.0/ or get it from GitHub: https://github.com/wxWidgets/wxWidgets

Further instructions on wxWidgets, read Building with wxErlang

##### Building Documentation

* xsltproc -- A command line XSLT processor.
A tool for applying XSLT stylesheets to XML documents. Download xsltproc from http://xmlsoft.org/XSLT/xsltproc2.html.

* fop -- Apache FOP print formatter (requires Java). Can be downloaded from http://xmlgraphics.apache.org/fop.

#### Steps

1. Download source code of erlang/otp 19
[https://github.com/erlang/otp/releases](https://github.com/erlang/otp/releases)

2. Install prerequired tools
 ```bash
    $ sudo apt-get insall gcc g++ m4 sed 
    $ sudo apt-get install openssl wx-common wx3.0-headers xsltproc fop
 ```
3. Uncompress the source code file and compile the code
  ```bash
   $ tar -xvf ${download_dir}/otp-OTP-19.tar.gz 
   $ cd otp-OTP-19
   $
  ```



