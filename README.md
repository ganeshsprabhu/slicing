Installation Steps:
sudo apt-get install opam
opam init
eval $(opam env --switch=default)
opam install frama-c
sudo apt install ocaml-dune
eval $(opam env)
Source : https://frama-c.com/html/get-frama-c.html

Slicing command used: frama-c sample_prg1.c -slice-value temperature  -then-on 'Slicing export' -print -ocode slice.c
doc: https://frama-c.com/fc-plugins/slicing.html
