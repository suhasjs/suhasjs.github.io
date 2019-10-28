---
title: "DiskANN: Fast Accurate Billion-point Nearest Neighbor Search on a Single Node"
collection: publications
permalink: /publication/diskann-neurips
excerpt: 'Current state-of-the-art approximate nearest neighbor search (ANNS) algorithms
generate indices that must be stored in main memory for fast high-recall search.
This makes them expensive and limits the size of the dataset. We present a
new graph-based indexing and search system called DiskANN that can index,
store, and search a billion point database on a single workstation with just 64 GB
RAM and an inexpensive solid-state drive (SSD). Contrary to current wisdom,
we demonstrate that the SSD-based indices built by DiskANN can meet all three
desiderata for large-scale ANNS: high-recall, low query latency and high density
(points indexed per node). On the billion point SIFT1B bigann dataset, DiskANN
serves > 5000 queries a second with < 3 ms mean latency and 95%+ 1 -recall @1
on a 16 core machine, where state-of-the-art billion-point ANNS algorithms with
similar memory footprint like FAISS and IVFOADC+G+P plateau at
around 50% 1-recall @1 . Alternately, in the high recall regime, DiskANN can
index and serve 5 − 10x more points per node compared to state-of-the-art graph-
based methods such as HNSW and NSG. Finally, as part of our overall
DiskANN system, we introduce Vamana , a new graph-based ANNS index that is
more versatile than the existing graph indices even for in-memory indices.'
date: 2019-12-08
venue: 'Neural Information Processing Systems (NeurIPS)'
paperurl: /files/diskann_neurips19.pdf
citation: 'Suhas Jayaram Subramanya, Devvrit, Rohan Kadekodi, Harsha Vardhan Simhadri, and Ravishankar Krishaswamy. "DiskANN: Fast Accurate Billion-point Nearest Neighbor Search on a Single Node". In *Advances in Neural Information Processing Systems (NeurIPS) 2019*'
---