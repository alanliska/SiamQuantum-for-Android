# This is the Siam Quantum fork used in the mobile app SiamQuantum

## Changes in this fork

* added the stamp defining the release (sq.c)
* option.c: added the include file <xc_funcs.h> from LIBXC
* dft.c: moved the block double g and double dgdrs
* Siam Quantum binaries are newly linked with libopenblas.a (without Fortran), therefore it is possible to use the official Android NDK´s clang as well as the GNU GCC based Android toolchains

## Compilation

open the Makefile
edit the paths to cross-compilers and precompiled dependencies (OPENBLAS, LIBXC)

```bash
$ make 
```

# ORIGINAL DESCRIPTION:

# Siam Quantum

*This GitHub repository is for source code, documentation, and reporting issues.* To download executables, please visit the official website: [https://sites.google.com/site/siamquantum](https://sites.google.com/site/siamquantum)

**Siam Quantum (SQ)** is a compact open-source quantum simulation program, designed for research and education in mind. For research, its speed and accuracy are comparable to the well-established quantum chemistry programs. You could use it to do research and publish your results with confident that your results can be reproduced. For education, it is extensively documented in an easy-to-read math display using Jupyter Notebook which can also be viewed directly on GitHub.

## 1. Executables

You could download the executables for MacOS, Linux, and Windows from the official website.

## 2. Compiling SQ

LAPACK library is required to build SQ from source code. It should be easy to build LAPACK using a fortran compiler. Optionally, LIBXC library can be called, granting access to other exchange-correlation functionals such as B3LYP, and PBE. 

### 2.1 Compiling LAPACK

#### 2.1.1 Using Linx/MacOS

#### 2.1.2 Using Windows


### 2.2 Compiling LIBXC



