Bos — Light, basic OS interaction for OCaml
-------------------------------------------------------------------------------
Release %%VERSION%%

Bos is an OCaml library providing basic tools for interacting with the
operating system. It provides tools to manipulate file paths,
execute commands and handle errors. Bos can be seen as an enhanced
`Sys` module for scripts and command line programs with light OS
interaction requirements. 

Bos depends on [Rresult][1] and is distributed under the BSD3 license. The
optional Bos_unix library depends on OCaml's Unix library.

[1]: http://erratique.ch/software/rresult

Home page: http://erratique.ch/software/bos  
Contact: Daniel Bünzli `<daniel.buenzl i@erratique.ch>`

## Installation

Bos can be installed with `opam`:

    opam install bos           # Base library
    opam install base-unix bos # Optional Unix support

If you don't use `opam` consult the [`opam`](opam) file for build
instructions.

## Documentation

The documentation and API reference is automatically generated by
`ocamldoc` from the interfaces. It can be consulted [online][5]
and there is a generated version in the `doc` directory of the
distribution.

[5]: http://erratique.ch/software/bos/doc/


## Sample programs

If you installed Bos with `opam` sample programs are located in
the directory `opam config var bos:doc`.

In the distribution sample programs are located in the `test`
directory of the distribution. They can be built with:

    ocamlbuild -use-ocamlfind test/tests.otarget

The resulting binaries are in `_build/test`.

- `test.native` tests the library, nothing should fail.
