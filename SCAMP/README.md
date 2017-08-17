## SCAMP

Since 3.10, [ATLAS](http://math-atlas.sourceforge.net) combined the "libcblas,
 libptcblas, libatlas" into two fat "libsatlas" and "libtatlas". This patch
 enables the software detect and compile with the latest ATLAS library.

This patch is a modified version based on the patch for SExtractor.

Phenomenon:

```configure: error: CBLAS/LAPack library files not found at usual locations! Exiting.```

Status: Author losing contact

Website: https://www.astromatic.net/software/scamp

Author: Emmanuel Bertin

Patch against:
 https://www.astromatic.net/download/scamp/scamp-2.0.4.tar.gz
