# SVG Embeded Image XLink Tests

Test cases for xlinked images in embedded SVGs.

## How to get started

[Raster tests](index.html)
[Vector tests](index-vector.html)

## How it works

My test SVGs have two layers:

* A bottom layer with a vector red X
* A top layer, with an embedded image, either a raster or vector green tick

A browser that renders the test correctly will only ever show the tick. A browser that fails the test will fail to display the tick, and show either the cross, or something else entirely.

## Test results

[Test results](test-results.md)

## How this came about

I was working with SVG images as part of layout development, and got pretty frustrated when I found that a feature that should have been obviously available as part of the regular SVG suite was non-functional across practically every environment. Here's a series of tweets I posted during the discovery phase.

> okay, someone out there has to have tried using a svg as a background image with an xlink to a jpeg in it. surely. anyone?

> i don't think it IS possible to use a raster image linked from a svg background image. tried safari, chrome, firefox; all failed. yay!

> bonus round: displaying an svg with xlinked images as an <img> element doesn't work either. the xlinked images just will not show.

> the only reliable way to display raster images inside an svg on the web is by embedding the entire svg inline.

> i'm sure there's a good reason for this, probably security-related, but what a crappy developer experience. carn @w3c, sort it out

> @w3c seriously, let me know if you want me to write up some test cases. this situation's crying out for improvement.

It was at this point that a W3C member got in contact with me and encouraged me to hurry up and write said test cases. I couldn't pass that up.
