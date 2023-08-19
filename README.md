# Exact Distributed Stochastic Block Partitioning (EDiSt)

Contains code relating to the "Exact Distributed Stochastic Block Partitioning" by F. Wanye, V. Gleyzer, E. Kao and W. Feng, which was accepted for publication to the 2023 IEEE Cluster conference. A [preprint is available on arXiv](https://arxiv.org/abs/2305.18663).

Stochastic block partitioning (SBP) code based on the reference implementation in the [Graph Challenge](http://graphchallenge.org)

Sequential, shared memory parallel, and distributed memory, multi-node parallel SBP code (EDiSt) is in src/main.cpp.

A C++ translation of the divide-and-conquer approach based on [iHeartGraph's implementation](https://github.com/iHeartGraph/GraphChallenge) and [Scalable Stochastic Block Partition paper](https://ieeexplore.ieee.org/document/8091050) is found in src/DivideAndConquerSBP.cpp.

The following steps should be sufficient to run the software on most unix systems:
```
git clone --recursive https://github.com/vtsynergy/EDiSt.git
cd EDiSt
mkdir build
cd build
cmake ..
make
./EDiSt --help
./DivideAndConquerSBP --help
```

# LICENSE 

&copy; Virginia Polytechnic Institute and State University, 2023.

Please refer to the included [LICENSE](./LICENSE) file.
