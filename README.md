# Godot Math Plot addon
A simple graph addon for godot to display math equations and scatter plots, called `MathPlot`

## Install
Create an folder called `addon` in the top of your projects directory then put these files into it.

## Functions:
- createSimpleLine(...) - takes a list of Vector2's and turns it into a line plot
- createScatterPlot(...) - takes a list of Vector2's and turns it into a bunch of dots
- createLabels(...) - takes an array of dictionaries of {"label": ..., "pos": Vector2(...), "color": Color...} and draws the strings on the graph

## Signals
The only signal is the `mouse_click` signal, which outputs where the mouse clicked in the graphs coordinate system.

## Export
plot_extent takes 2 Vector2's:
 - The first Vector2 represents the bottom left corner of your coordinate system
 - The second Vector2 represents the top right corner of your coordinate system

grid_spacing is a Vector2 which specifies how big the ticks along each axis should be

spline_length governs how "smooth" your line plots will be, this is mostly set by eye

## Heads Up
Don't forget to call update(), no changes will be drawn until done so

### Thanks
[Big thanks to  Dlean Jeans for the SmoothPath addon](https://godotengine.org/qa/32506/how-to-draw-a-curve-in-2d)

[Thanks to maciek134 for the rangef function as well](https://github.com/godotengine/godot/issues/4164#issuecomment-488754325)
