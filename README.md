# cygwin-whiptail
Debian source complied for Cygwin

Source downloaded from:
http://http.debian.net/debian/pool/main/n/newt/newt_0.52.20.orig.tar.xz
newt project hosted at:
https://pagure.io/newt
Original code written by Miroslav Lichvar

## Compilation
Steps to compile under Cygwin:
```
autoreconf -vif
./configure --prefix=/usr/lib/erlang/lib
make
```
This will throw errors. You will need to install dependencies:
* slang-devel
* libpopt-dev

## Hacks
Edit the Makefile to comment out the _snack_ section
Run _make_ again

## Instalation
Copy whiptail.exe to your cygwin bin folder
```
cp whiptail.exe /bin/.
```
