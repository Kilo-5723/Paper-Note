# Mining Bursting Core in Large Temporal Graphs

VLDB 2022
;
[paper link](https://www.vldb.org/pvldb/vol15/p3911-wang.pdf)

Keyword: Bursting Core

## Summary

### Problem Statement

Degree Sequence: A sequence of some node's sequence in each snapshot of the temporal graph.

$l$-Segment Density: The average degree of some node's degree sequence while the length of the segment is no less than $l$.

$(l,\delta)$-Bursting Node: A node where maximum segment density is greater than $\delta$.

Pareto-optiomal $(l,\delta)$-maximal bursting core: Maximal bursting cores that are not dominated by other $(l,\delta)$-maximal bursting cores.

The problem is to mine maximal bursting cores in a temporal graph.

### Soultion

- Baseline: Decomposition algorithm to mine the maximal bursting core
- Optimization 1: Use dynamic programming algorithm to compute setment density more efficiently.
- Optimization 2: Prune useless MSD calculation.

## Strong Point

- This algorithm has a tight timebound, and the experiment shows that the pruning can make it even more faster in practice.
- The figures in the experiment section shows the effectiveness of this algorithm clearly.