![Thesaurus](./resources/asplos.png)

In this paper, we identify a previously untapped source of compressibility in cache working sets: clusters of cachelines that are similar, but not identical, to one another.
 To compress the cache, we can then store the "clusteroid" of each cluster together with the (much smaller) "diffs" needed to reconstruct the rest of the cluster.
 To exploit this opportunity, we propose a hardware-level on-line cacheline clustering mechanism based on locality-sensitive hashing.
 Our method dynamically forms clusters as they appear in the data access stream and retires them as they disappear from the cache.
 Our evaluations show that we achieve 2.25× compression on average (and up to 9.9×) on SPECCPU 2017 suite and is significantly higher than prior proposals scaled to an iso-silicon budget.


##
Main classes: please refer to `approximatededupbdi_cache.h` and `approximatededupbdi_cache.cpp`


# Cache Compression zsim
This is a variation of the original [zsim simulator](https://github.com/s5z/zsim) that supports compressed caches. For more details please see [here](README_zsim.md).
