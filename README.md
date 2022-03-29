# Test models for the butterfly-LBO repository

This repository contains some test models for the [https://github.com/sampotter/butterfly-LBO](butterfly-LBO) repository, which pulls inclues it as a submodule, and is backed by GitHub's Git LFS support.

The naming convention of the included files is `name<n>.ext`, where `n` is a nonnegative integer. The values `n = 0, ..., nmax` should be represented. The model indexed by `nmax` is the original, undecimated model. Each successively smaller value of `n` is a decimated version of `name<nmax>.ext`, done using MeshLab's "quadric edge collapse decimation" filter. The result is a sequence of meshes, each with about half as many vertices and faces as the last. The final mesh (with `n == 0`) has a small-ish number of vertices (a few thousand at most).
