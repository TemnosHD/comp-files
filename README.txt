## Manual for the experimental GCC-PPU backend ##

things to do:

1.)
get gcc-4.9.2, linux-3.17.2, binutils-2.25, glibc-2.20, mpfr-3.1.2, gmp-6.0.0a, mpc-1.0.2, isl-0.12.2, cloog-0.18.1
and unzip everything in your source directory

2.)
get the repo https://github.com/TemnosHD/rs6000
copy the above repo to gcc-4.9.2/gcc/config/rs6000/

3.)
run 'update-cross-comp'
the commented lines are typically not needed, incase the compiler claims you are trying to initialze an unrpototyped function -> uncomment lines 79-115

4.)
'source load-exp-gcc.sh'

5.)
in the nux folder, modify main.c and run 'make clean test0'
