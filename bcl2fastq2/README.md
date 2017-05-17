## bcl2fastq2

* Since Boost 1.56.0, the Boost Xml module has changed its calling conversion,
 thus need explicit type hint.

* On Gentoo platform, 'OF' macro of zlib is renamed to '\_Z\_OF'.
 A tweak is applied to make 'OF' an alias to '\_Z\_OF' if it is not defined.

Status: Pushing to upstream

Website:
 https://support.illumina.com/sequencing/sequencing_software/bcl2fastq-conversion-software.html

Author: Illumina, Inc.

Patch against:
 https://support.illumina.com/content/dam/illumina-support/documents/downloads/software/bcl2fastq/bcl2fastq2-v2.19.0.tar.gz
