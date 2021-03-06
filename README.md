# Java Vector API SIMD benchmark
This example utilizes the [SIMD capabilities](https://blogs.oracle.com/javamagazine/post/java-vector-api-simd) ([SSE](https://www.intel.com/content/www/us/en/support/articles/000005779/processors.html) or [AVX](https://www.intel.com/content/www/us/en/support/articles/000005779/processors.html) / [Neon](https://developer.arm.com/architectures/instruction-sets/simd-isas/neon) or [SVE](https://developer.arm.com/tools-and-software/server-and-hpc/compile/arm-instruction-emulator/resources/tutorials/sve) extensions) of contemporary x86 and ARM CPUs through a [simple array averaging example](app/src/main/java/hu/laszlolukacs/vectorsimdbench/ArrayAverageCalculator.java) using the Java [Vector API (JEP 338)](https://openjdk.java.net/jeps/338).

## Dependencies ##
* [JDK 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html) or newer

## System Requirements ##
* *x64* or *AArch64* CPU with SIMD instructions (*SSE* or *AVX* extensions on `x64_64`, *Neon* or *SVE* extensions on `AArch64`) running a supported **64-bit** version of Linux, macOS or Windows OS
* [JRE 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html) or newer

## Summary of set up
* `git clone git@github.com:laszlolukacs/vector-simd-in-java-benchmark.git`
* `cd ./vector-simd-in-java-benchmark`
* `gradle build`

## Basic Usage
* Invoke `gradle runtimeBenchmark` from repo root
