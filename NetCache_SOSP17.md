# Title: NetCache: Balancing Key-Value Stores with Fast In-Network Caching

[Xin Jin et al. SOSP'17](doi.org/10.1145/3132747.3132764)

# Author:
Xin Jin, Xiaozhou Li, Haoyu Zhang, Robert Soulé, Jeongkeun Lee, Nate Foster, Changhoon Kim, and Ion Stoica

# Summary
Authors propose an in-network caching scheme for key-value store (KVS) tuples.
Their architecture is built upon a programmable dataplane (Tofino). The dataplane componentes include the KVS cache and a mechanismo to detect
potential new hot items based on a count-min sketch and a bloom filter. The dataplane components are written in P4.
The performance improvement is up to 10x in terms of throughput and the latency is reduced by up to 50%, despite the relatively low hit-ratio (<50 %).

## Insights

Cache coherence uses write-through.
Not sure why a sketck plus a bloom was used. Need check if HashPipe guarantees removing duplicates.
Hot items are reported to the controller periodically (1 s interval) with refresh.
Authors report limitations of programmable dataplanes. Some manual mapping is needed in order to make things work properly.
Authors comment on heterogenous platform for distributed systems (prog DP + server).
Test set generated using a zipf distribution.

## Processing Algorithm

    if read
      if in cache
        read and update statitics
      else
        update heavy hitter
        report hot items
    else
      invalidade cache entry

