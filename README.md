# FluidType
Simple test with fluid type and ~~molten leading~~.

Molten leading proves difficult as Firefox doesn’t accept `calc` for line-heights. So we got to stick to the same `line-height` that we first define. It still gets processed but then recalculated to `rem`, this is purely to force a repaint in Safari.
