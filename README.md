# SVG Embeded Image XLink Tests

Test cases for xlinked images in embedded SVGs.

## How to get started

[Raster tests](https://rtrvrtg.github.io/svg-embed-xlink-tests/index.html)
[Vector tests](https://rtrvrtg.github.io/svg-embed-xlink-tests/index-vector.html)

## How it works

My test SVGs have two layers:

* A bottom layer with a vector red X
* A top layer, with an embedded image, either a raster or vector green tick

A browser that renders the test correctly will only ever show the tick. A browser that fails the test will fail to display the tick, and show either the cross, or something else entirely.

## Test results

[Test results](test-results.md)
