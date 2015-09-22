# Java Linpack Benchmark

Java Linpack Benchmark is a translation of the popular Linpack benchmark, originally written in Fortran. The Benchmark is a numerically intensive test that has been used for years to measure the floating point performance of computers.

To see more about the project, visit:
http://www.netlib.org/benchmark/linpackjava/


## How to use

Compile by run:

    javac -O Linpack.java

To run:

    java Linpack

## Notes

"""Modified 3/3/97 by David M. Doolin (dmd) doolin@cs.utk.edu
Fixed error in matgen() method. Added some comments.

Modified 1/22/97 by Paul McMahan mcmahan@cs.utk.edu
Added more MacOS options to form.

Optimized by Jonathan Hardwick (jch@cs.cmu.edu), 3/28/96
Compare to Linkpack.java.
Optimizations performed:

 - added "final" modifier to performance-critical methods.
 - changed lines of the form "a[i] = a[i] + x" to "a[i] += x".
 - minimized array references using common subexpression elimination.
 - eliminated unused variables.
 - undid an unrolled loop.
 - added temporary 1D arrays to hold frequently-used columns of 2D arrays.
 - wrote my own abs() method

See http://www.cs.cmu.edu/~jch/java/linpack.html for more details.


Ported to Java by Reed Wade  (wade@cs.utk.edu) 2/96
built using JDK 1.0 on solaris
using "javac -O Linpack.java"


Translated to C by Bonnie Toy 5/88
  (modified on 2/25/94  to fix a problem with daxpy  for
   unequal increments or equal increments not equal to 1.
     Jack Dongarra)
"""