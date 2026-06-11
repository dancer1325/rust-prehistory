This is preliminary version of the Rust compiler.

# [boot](boot)
* == Bootstrap compiler
* [boot/fe](boot/fe)
  * FE
  * == MULTIPLE components
    * lexer
      * == TODO:  
    * parser
      * == TODO:
    * AST
      * == TODO:
* [boot/me](boot/me)
  * TODO: Middle end (resolve, check, layout, trans)
* [boot/be](boot/be)
  * -- based on -- OCaml
  * == MULTIPLE components
    * IL
      * == Intermediate Language
    * RA
      * == Register Allocation
    * insns
      * == Instructions
    * asm
      * == Assembly
    * objfiles
      * == Object files
* [boot/util](boot/util)
  * Ubiquitous helpers
* [boot/llvm](boot/llvm)
  * LLVM-based alternative back end
* [boot/driver](boot/driver)
  * Compiler driver

# [comp](comp)
  * Self-hosted compiler (doesn't exist yet)
  * Same structure as in boot/

# [rt](rt)
  * Runtime system
  * rt/rust_*.cpp
    * The majority of the runtime services
  * [rt/isaac](rt/isaac)
    * PRNG used for pseudo-random choices in the runtime
  * [rt/bigint](rt/bigint)
    * Bigint library used for the 'big' type
  * [rt/uthash](rt/uthash)
    * Small hashtable-and-list library for C, used in runtime
  * [rt/sync](rt/sync), [rt/util](rt/util)
    * Small utility classes for the runtime

# [test](test)
  * Testsuite (for both bootstrap and self-hosted)
  * [test/compile-fail](test/compile-fail)
    * Tests that should fail to compile
  * [test/run-fail](test/run-fail)
    * Tests that should compile, run and fail
  * [test/run-pass](test/run-pass)
    * Tests that should compile, run and succeed
