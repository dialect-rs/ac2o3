# Ac<sub>2</sub>O<sub>3</sub>
[![CI](https://github.com/dialect-rs/ac2o3/actions/workflows/CI.yml/badge.svg)](https://github.com/dialect-rs/ac2o3/actions/workflows/CI.yml)


Rust implementation of an Anderson Acceleration algorithm based on Ref [1].<br>
Please note: There is an original [Matlab implementation](https://web.stanford.edu/~boyd/papers/nonexp_global_aa1.html)
as well as a slightly modified [implementation in C](https://www.cvxgrp.org/scs/algorithm/acceleration.html) (including 
a Python interface) by the authors of the paper.<br>
Ac<sub>2</sub>O<sub>3</sub> is a port of the C implementation to Rust.

### Dependencies
Building Ac<sub>2</sub>O<sub>3</sub> requires the following to be installed: 
- OpenBLAS: <br>
On linux systems you can either install it by just executing `sudo apt-get install libopenblas-dev` or follow 
the instructions on the [repository page](https://github.com/xianyi/OpenBLAS).
On macOS OpenBLAS can be installed using [HomeBrew](): `brew install openblas`. Make sure that the homebrew path is 
 included in `$LIBRARY_PATH`. So you might need to execute: <br>
  `export LIBRARY_PATH=/opt/homebrew/Cellar/:$LIBRARY_PATH` (on Apple Silicon/M1 processors)<br>
  `export LIBRARY_PATH=/usr/local/Cellar/:$LIBRARY_PATH` (on Intel processors)<br>

  
### References:<br>
<hr>
[1]: J. Zhang, B. O'Donoghue, and S. Boyd, <a href="https://web.stanford.edu/~boyd/papers/pdf/scs_2.0_v_global.pdf">Globally
  Convergent Type-I Anderson Acceleration for Non-Smooth Fixed-Point Iterations</a>, 30(4):3170–3197, 2020. 
SIAM Journal on Optimization


#### License

<sup>
Licensed under either of <a href="LICENSE-APACHE">Apache License, Version
2.0</a> or <a href="LICENSE-MIT">MIT license</a> at your option.
</sup>

<br>

<sub>
Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in this crate by you, as defined in the Apache-2.0 license, shall
be dual licensed as above, without any additional terms or conditions.
</sub>