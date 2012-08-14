This project aims to provide the online supplement for *Constrained Min-Cut
Replication for K-Way Hypergraph Partitioning* article. Repository contains the
experimented data, partitioning and replication results. Further, an interactive
HTML report summarizing the results is located at
[http://vy.github.com/cmcr](http://vy.github.com/cmcr) address.

Repository contents are structured as follows.

* `data` directory contains the hypergraphs. For instance,
  `data/ir/Facebook.patoh` file provides the *Facebook* hypergraph in PaToH
  format and it is classified under *information retrieval* (`ir`) data set.
  `data/ir/Facebook.patoh.info` contains properties of the same hypergraph.

* `part` directory contains the hypergraph partitions that are used in the
  conducted experiments. For example, `part/ir/Facebook/k128/Facebook.part`
  contains the partitioning results for *Facebook* hypergraph, where number of
  parts are set to 128, i.e., *K=128*.
  `part/ir/Facebook/k128/Facebook.part.info` and
  `part/ir/Facebook/k128/Facebook.part.prof` contains the corresponding
  partition properties and profiling results, respectively.

* `repl` directory contains the replication results. For instance,
  `repl/o1/ir/Facebook/k128/r0.10/t1/dm/Facebook.repl` file provides the
  replication results for *Facebook* hypergraph partition, where

  * `o1` denotes that the first ordering scheme is used,
  * `ir` denotes that this is an *information retrieval* data set,
  * `k128` denotes that *K=128*,
  * `r0.10` denotes that *&#961;=0.10*,
  * `t1` denotes that *&#120514;=1*, and
  * `dm` denotes that the Dulmage-Mendelsohn coarsening scheme is used.

  Likewise, `repl/o1/ir/Facebook/k128/r0.10/t1/dm/Facebook.repl.prof` contains
  the profiling results for the corresponding replication.

  If there exists an `.error` file (e.g.,
  `repl/o1/ir/Facebook/k256/r0.20/t4/patoh_mnc/Facebook.repl.error`), it means
  that there occurred an internal error (e.g., not sufficient memory) during
  replication.
