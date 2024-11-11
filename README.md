# Installation Steps

To install the required tools, follow the steps below:

```bash
sudo apt-get install opam
opam init
eval $(opam env --switch=default)
opam install frama-c
sudo apt install ocaml-dune
eval $(opam env)


frama-c sample_prg1.c -slice-value temperature -then-on 'Slicing export' -print -ocode slice.c
