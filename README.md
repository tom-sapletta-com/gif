# gif
animiation, resize, screen saver

## Terminalizer
https://github.com/faressoft/terminalizer
Record your terminal and generate animated gif images or share a web player

### Installation
You need to install Node.js first, then install the tool globally using this command:

    npm install -g terminalizer

### Getting Started
Start recording your terminal using the record command.

    terminalizer record demo

A file called demo.yml will be created in the current directory. You can open it using any editor to edit the configurations and the recorded frames. You can replay your recording using the play command.

    terminalizer play demo

### Now let's render our recording as an animated gif.

    terminalizer render demo


## Server side images and animations generation with node
http://jeremybouny.fr/en/articles/server_side_canvas_node/

## GIF streaming
https://github.com/pkrumins/node-gif

 produce GIF images from RGB, BGR, RGBA or BGRA buffers.

This module exports Gif, DynamicGifStack, AnimatedGif and AsyncAnimatedGif objects.
Gif

The Gif object is for creating simple GIF images. Gif's constructor takes takes 5 arguments:

var gif = new Gif(buffer, width, height, quality, buffer_type);

The first argument, buffer, is a node.js Buffer that is filled with RGB, BGR, RGBA or BGRA values. The second argument is integer width of the image. The third argument is integer height of the image. The fourth argument is the quality of output image. The fifth argument is buffer type, 'rgb', 'bgr', 'rgba' or 'bgra'.

You can set the transparent color for the image by using:


## Resizing, GIF Animation with gifsicle
http://www.lcdf.org/gifsicle/

a few easy methods for resizing a GIF with gifsicle:

### Scaling of an image - 50%
gifsicle --scale 0.5 -i animation.gif > animation-smaller.gif

### Scale to a given width with unspecified height
gifsicle --resize-fit-width 300 -i animation.gif > animation-300px.gif

### Scale to a given height with unspecified width
gifsicle --resize-fit-height 100 -i animation.gif > animation-100px.gif

### Clip to size
gifsicle --resize 300x200  -i animation.gif > animation-clipped.gif

You can use scale to easily scale an image by a given factor, but you can also use --resize-fit-height or --resize-fit-width to scale to respective sizes.  You can also clip with --resize. 
