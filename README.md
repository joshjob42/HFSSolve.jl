# HFSSolve

[![Build Status](https://travis-ci.org/joshjob42/HFSSolve.jl.svg?branch=master)](https://travis-ci.org/joshjob42/HFSSolve.jl)

A little repo to work on a generic Hamze-Freitas-Selby solver for an arbitrary graph structure with nodes of arbitrary dimension. There'll need to be some mapping work to go from ProblemInstances and similar things into the full Graphs.jl type graph used here (though perhaps a simple dictionary of tuples [(i,j)=>J_ij] might be sufficient to represent the problem). Users will have to supply the trees to run over directly and either provide an order or trees will be chosen at random from the provided set.