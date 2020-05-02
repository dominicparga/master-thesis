# Notes

These notes contain todos and plans up to submission at `June 19th, 2020`.

## Planning

Some things have to be done in a specific order or time, while some other things are just nice-to-haves or it is unclear, whether they are needed at all.

- __TODO 00__: implement algorithm for finding best alpha-routes given a CH-graph from [multi-ch-constructor][github/lesstat/multi-ch-constructor] -> 3 components (see [cyclops][github/lesstat/cyclops] and [`CRTP`][fluentcpp/crtp])
  - CH-Dijkstra, first without using sweep-algorithm due to uncontracted nodes and hence special treatment
    - bidirectional Dijkstra going upwards in node-level (>=, not >, for correctness when using one level for all nodes)
  - LGS (there should exist a crate for this)
  - working with convex hull -> [nd-triangulation][github/lesstat/nd-triangulation]
- __TODO 01__: evaluating and iterating/learning new metrics
- __TODO 02__: visualization
  - Use [geojson][github/dominicparga/howto/issues/36]?
- CH-explanation: [fmi-pdf][uni-stuttgart/fmi/ch]
  - improve query-time (up to 10x) using `stall-on-demand`, see [here][uni-stuttgart/fmi/ch].
- Route generation
  - ~ 1k s-t-pairs, each with alternative routes
  - det. f. graph + constraints -> datastructure: set
  - save in intermediate format?
  - forall s-t-pairs : choose an alternative route
- Graph -> `JSON`, possibly with reduction using `GzEncoder` from crate `flate2` if too expensive in performance

## Paper-content

- Good points:
  - Routing is more system-dependent than with dynamic routing, which allows improving the system more immediate, not the routing.
  - Dynamic routing is not that good if network-units (like drivers) can't be watched directly.
    In other networks, packages can only be watched indirectly, at nodes, which could cost performance, if every node is just looking for its local best solution, where a global solution would be better.
    If routing-algorithms would lead to better global results, this performance-issue could be improved.

## Tips

- When writing paper, always write and extend it in breadth, not in depth.

[fluentcpp/crtp]: https://www.fluentcpp.com/2017/05/12/curiously-recurring-template-pattern/
[github/dominicparga/howto/issues/36]: https://github.com/dominicparga/howto/issues/36
[github/lesstat/cyclops]: https://github.com/lesstat/cyclops
[github/lesstat/multi-ch-constructor]: https://github.com/lesstat/multi-ch-constructor
[github/lesstat/nd-triangulation]: https://github.com/lesstat/nd-triangulation
[uni-stuttgart/fmi/ch]: https://fmi.uni-stuttgart.de/files/alg/teaching/s15/alg/CH.pdf
