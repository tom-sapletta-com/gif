# gif
animiation, resize, screen saver

# GIF Animation with gifsicle
http://www.lcdf.org/gifsicle/

a few easy methods for resizing a GIF with gifsicle:

# Scaling of an image - 50%
gifsicle --scale 0.5 -i animation.gif > animation-smaller.gif

# Scale to a given width with unspecified height
gifsicle --resize-fit-width 300 -i animation.gif > animation-300px.gif

# Scale to a given height with unspecified width
gifsicle --resize-fit-height 100 -i animation.gif > animation-100px.gif

# Clip to size
gifsicle --resize 300x200  -i animation.gif > animation-clipped.gif

You can use scale to easily scale an image by a given factor, but you can also use --resize-fit-height or --resize-fit-width to scale to respective sizes.  You can also clip with --resize. 
