# Some random benchmark for M1 macbook
## Machines
* MacBook Air (M1, 2020), 16GB Mem
* MacBook Pro (16-inch, 2019), 2.4 GHz 8-Core Intel Core i9, 32GB Mem
* i7-6700K CPU @ 4.00GHz, 32GB Mem Desktop on Ubuntu 18.04.5 LTS x86_64

## Benchmarks
### CHOLMOD Demo, SuiteSparse 5.8.1
* MacBook Air (M1, 2020)
```
./cholmod_l_demo nd6k/nd6k.mtx > nd6k.m1.txt  9.83s user 0.52s system 164% cpu 6.293 total
```
* MacBook Pro (16-inch, 2019)
  * default
  ```
  ./cholmod_l_demo nd6k/nd6k.mtx > nd6k.i9.txt  32.86s user 3.30s system 394% cpu 9.164 total
  ```
  * w/ mkl
  ```
  ./cholmod_l_demo nd6k/nd6k.mtx > nd6k.i9.txt  34.17s user 3.45s system 406% cpu 9.251 total
  ```
  * w/ openblas
  ```
  ./cholmod_l_demo nd6k/nd6k.mtx > nd6k.i9.txt  33.90s user 3.85s system 400% cpu 9.419 total
  ```
* i7 Desktop
  * w/ openblas
  ```
  time ./cholmod_l_demo nd6k/nd6k.mtx > nd6k.i7.txt

  real	0m14.627s
  user	1m6.857s
  sys	0m30.580s
  ```
