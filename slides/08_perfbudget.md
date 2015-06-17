<!-- .slide: data-background="images/6097066382_e4f07e8a75_o.jpg" -->
<div class="attribution">Photo: [flickr/teegardin](https://www.flickr.com/photos/teegardin/6097066382/)</div>

# Performance budgets

--

#### It’s easier to make a fun game fast<br>than it is to make a fast game fun.<br> (Robert Nystrom)

But we still have to make it fast.

Note:
but a game must still be fast

--

<!-- .slide: data-background="images/53d7ad732fafc.png" -->
<div class="attribution">Photo: [rcwebdev.co.uk](http://www.rcwebdev.co.uk/view-portfolio/c64-loading-screen-simulator)</div>


# Time based budgets

- Startup time
- Load time, level transition time

Note:
web development has this budget

--

<!-- .slide: data-background="images/5187446637_613eb6763e_o.jpg" -->
<div class="attribution">Photo: [flickr/schtumple](https://www.flickr.com/photos/schtumple/5187446637/)</div>

# Per frame

60 frames per second &#x2248; 16.66667 ms per frame

--

# Hardware based
- Memory footprint
- Network (bandwidth, latency)
- Power consumption (phones, tablets, laptops)

--

### Testing is made easier

## within or out of budget?

--

## Dealing with new features
Does feature X fit into the performance budget?

--

# What can be removed instead?

Note: what are we willing to pay for it?

--

# Example

| | |
|-|-|
| Feature	| A new web font is needed for some fancy headlines
| Budget	| Website needs to load fast, Page speed index must stay under 1000
| Before	| Speed index 980
| After		| Speed index 1320
| Conclusion| It doesn't fit. Can something else be removed? Is it worth to "overspend"?

Note:
- Negotiation begins...
- Feature maybe only for desktop devices?
