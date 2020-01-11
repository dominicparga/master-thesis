# Notes

These notes contain todos and plans up to submission at `June 19th, 2020`.

## Planning

Some things have to be done in a specific order or time, while some other things are just nice-to-haves or it is unclear, whether they are needed at all.

- __TODO 00__: implement algorithm for finding best alpha-routes -> 3 components (see [cyclops][github/Lesstat/cyclops] and [`CRTP`][fluentcpp/crtp])
  - CH-Dijkstra
  - LGS (there should exist a crate for this)
  - working with convex hull -> [nd-triangulation][github/Lesstat/nd-triangulation]
- __TODO 01__: evaluating and iterating/learning new metrics
- __TODO 02__: visualization
  - Use [geojson][github/dominicparga/howto/issues/36]?
- Route generation
  - ~ 1k s-t-pairs, each with alternative routes
  - det. f. graph + constraints -> datastructure: set
  - save in intermediate format?
  - forall s-t-pairs : choose an alternative route
- Graph -> `JSON`, possibly with reduction using `GzEncoder` from crate `flate2` if too expensive in performance

## Tips

- When writing paper, always write and extend it in breadth, not in depth.

[fluentcpp/crtp]: https://www.fluentcpp.com/2017/05/12/curiously-recurring-template-pattern/
[github/Lesstat/cyclops]: https://github.com/Lesstat/cyclops
[github/Lesstat/nd-triangulation]: https://github.com/Lesstat/nd-triangulation
[github/dominicparga/howto/issues/36]: https://github.com/dominicparga/howto/issues/36
