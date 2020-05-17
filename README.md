# Lemon

https://www.sqlite.org/src/doc/trunk/doc/lemon.html

This project provides an installable version of latest `lemon`, as of when I put this together.

`lemon` learned how to put output files in an arbitrary directory around sqlite 3.31, however my distro packages an earlier version than that.

Extraction occured from:

git hash:    b2eb7e46eb3c0a1611d7777fb3a1ba9b30f56ea5

fossil hash: 55910b9a7287be92af9f95e0af54af822055d15b7eabbcc81d61410d0bf67726

though these files are both roughly 6 months older than that.

My only change is
```c
  static char templatename[] = LEMPAR; // previously "lempar.c"
```
in `tplt_open()`, which I set to the install destination in the build script.
