## SExtractor

Since 3.10, [ATLAS](http://math-atlas.sourceforge.net) combined the "libcblas,
 libptcblas, libatlas" into two fat "libsatlas" and "libtatlas". This patch
 enables the software detect and compile with the latest ATLAS library.

Phenomenon:

```configure: error: CBLAS/LAPack library files not found at usual locations! Exiting.```

Status: Author losing contact

Website: https://www.astromatic.net/software/sextractor

Author: Emmanuel Bertin

Patch against:
 https://www.astromatic.net/download/sextractor/sextractor-2.19.5.tar.gz
