## PGPLOT

Direct access to ```png_ptr->jmpbuf``` has been deprecated since
[libpng 1.4](http://www.libpng.org/pub/png/src/libpng-1.2.x-to-1.4.x-summary.txt). This patch allowed PGPLOT to compile with modern libpng.

Also provided configs (with patch demonstrate what I edited) for Intel compilers,
inspired by [Intel performance guide](https://software.intel.com/en-us/articles/performance-tools-for-software-developers-building-pgplot-with-the-intel-compilers/#buildingPGPLOT).

Phenomenon:

```make: *** No rule to make target `png.h', needed by `pndriv.o'.  Stop.```

```
../pgplot//drivers/pndriv.c:225:21: error: dereferencing pointer to incomplete type ‘png_struct’ {aka ‘struct png_struct_def’}
   if (setjmp(png_ptr->jmpbuf)) { /* not really sure what I'm doing here... */
                     ^~
```
or
```
../pgplot//drivers/pndriv.c(225): error: pointer to incomplete class type is not allowed
    if (setjmp(png_ptr->jmpbuf)) { /* not really sure what I'm doing here... */
        ^
```

Status: Pushing to upstream

Website: http://www.astro.caltech.edu/~tjp/pgplot/

Author: Tim Pearson

Patch against:
 ftp://ftp.astro.caltech.edu/pub/pgplot/pgplot522.tar.gz
