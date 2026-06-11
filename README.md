Rust Prehistory Repo - November 2016
====================================

* goal
  * reconstruction -- of the -- Rust "prehistory" development
    * [2006, 2009]
      * == personal project
    * [2009, 2010]
      * -- as -- Mozilla project / private

Documentation
----------

* [here](doc/notes)

Project
----------

* [here](src/README.md)

Edits made vs ORIGINAL
----------

1. Converted from Monotone and Mercurial revision control
2. Deleted [PDFs](PDFs.md) + other reference material
   * Reason:🧠NO right to redistribute🧠
3. Deleted commits OR files / too embarrassing OR too worthless to publish

Caveats (i.e. "don't expect much")
----------------------------------

* what was his process?
  * | study OTHER languages,
    * take notes
    * ways to approach DIFFERENT

Linking history in Git
----------------------

* if you want to browse the Rust project's FULL (ALSO FROM personal project) history  -> link this history -- with -- [active Rust repository](https://github.com/rust-lang/rust/)
  * steps
    * | Rust repository, 
     ```shell
     git remote add prehistory https://github.com/graydon/rust-prehistory.git
     git remote update prehistory
     git replace c01efc669f09508b55eced32d3c88702578a7c3e c10ce161d8a58d78e10583fcea7e34eab0a518d0
     ```
  * _Example:_ check the full history of "hello, world"

     ```shell
     git log -p --follow src/test/ui/hello.rs
     ```
