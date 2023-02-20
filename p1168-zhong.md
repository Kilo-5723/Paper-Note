# Scalable Time-Range $k$-Core Query on Temporal Graphs

VLDB 2023
;
[paper link](https://www.vldb.org/pvldb/vol16/p1168-zhong.pdf)

Keyword: Query on Temporal Graph

## Summary

### Problem Statement

This paper formalized a novel Temporal $k$-Core Query problem: given a time interval, find all distinct $k$-cores that exist within any subintervals from a temporal graph.

### Solution

- Baseline: Calculate $k$-core for each time interval.
- Optimization 1: Calculate the $k$-core of a time interval $[l,r]$ from the $k$-core of the time interval $[l-1,r]$ if it exists.
- Optimization 2: When the $k$-core of a time interval $[l,r]$ has a tighter time interval bound $[l',r']\subset [l,r]$, some time intervals can be pruned based on three rules given in Section 4.2.


## Strong Point

- The definition of the Temporal $k$-Core Query and the pruning used in this paper are both inspiring.
- The paper uses informative figures to explain the procedure of the algorithm.
- The tables used in the experiment section shows the effect of pruning detailedly.

## Weak Point

- The algorithm in this paper is rather simple.