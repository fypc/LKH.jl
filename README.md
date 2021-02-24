# LKH.jl

[![Build Status](https://github.com/chkwon/LKH.jl/workflows/CI/badge.svg?branch=master)](https://github.com/chkwon/LKH.jl/actions?query=workflow%3ACI)
[![codecov](https://codecov.io/gh/chkwon/LKH.jl/branch/master/graph/badge.svg)](https://codecov.io/gh/chkwon/LKH.jl)

This package provides a Julia wrapper for the [LKH solver](http://webhotel4.ruc.dk/~keld/research/LKH/) for solving Traveling Salesman Problems (TSP).  LKH is Keld Helsgaun's efficient implemtation of the Lin-Kernighan heuristic.

```julia
using LKH 

M = [
    0  16   7  14
   16   0   3   5
    7   3   0  16
   14   5  16   0 
]
opt_tour, opt_len = solve_tsp(M)
```
