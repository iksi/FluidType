# FluidType
Simple test with fluid type and ~~molten leading~~.

Molten leading proves difficult as Firefox doesn’t accept `calc` for line-heights. So we got to stick to the same `line-height` that we first define. It still gets processed but then recalculated to `rem`, this is purely to force a repaint in Safari.

Basic math behind it: (source: http://madebymike.com.au/writing/precise-control-responsive-typography)

```
calc(minSize + (maxSize - minSize) * ((100vw - minPort) / (maxPort - minPort)))
```

As stated above `line-height` cannot be increased/decreased because of Firefox, but Safari needs the `line-height` recalculated (even if it stays the same) to force the repaint of the `font-size`.
