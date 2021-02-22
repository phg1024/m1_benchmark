# Some random benchmark for M1 macbook
## Machines
* MacBook Air (M1, 2020)
* MacBook Pro (16-inch, 2019)

## Benchmarks
### SuiteSparse 5.8.1
* MacBook Air (M1, 2020)
```
./cholmod_l_demo nd6k/nd6k.mtx > nd6k.m1.txt  9.83s user 0.52s system 164% cpu 6.293 total
```
* Macbook Pro 
  * w/o mkl
  ```
  ./cholmod_l_demo nd6k/nd6k.mtx > nd6k.i9.txt  32.86s user 3.30s system 394% cpu 9.164 total
  ```
  * w/ mkl
  ```
  TBA
  ```
