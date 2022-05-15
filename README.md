# Curtain & Sync Modes for OpenSeadragon
===============

This library is an extension for [OpenSeadragon](https://openseadragon.github.io/#) and represents a modified version of https://github.com/cuberis/openseadragon-curtain-sync that enables side-by-side, synchronized image viewing.

This fork provides handles for additional layers with overlay controls as well as a visible 'nubbin' in the ui for controlling the position of the curtain.
It is part of a set of small tools that enable interaction between the sketchfab api (see sketchfab fade) and iiif images.

It is unlikely to work in it's current form without considerable work but may provide inspiration. Release of a content neutral demo is in **progress**.

Based on the original curtain sync plugin
**Curtain mode** overlays images on top of each other and reveals more or less of each image based on the position of the nubbin. Multiple images can be loaded into the stack, but only the first 2 are split in the curtain (a third is an option using original code) with later layers as full-viewer overlays that can have their opacity modified.

# Currently deprecated
**Sync mode** shows images side-by-side but keeps each image in sync as the user zooms or pans.

# Dependencies
--------------


This version of the viewer has a handle (called 'nubbin') to make touch screen use more intuitive.

The current version is built for an interface that has a single Open Sea Dragon viewing area, that swaps between multiple Open Sea Dragon viewer (for different items on the page).

The **nubbin**  must be placed within this container on the main page. E.g.

<div id="osd-container" blah blah.... >

   <div id="osd-viewer-0" class="container-fluid h-100 w-100 p-0 osdViewer"></div>
   <div id="osd-viewer-1" class="container-fluid h-100 w-100 p-0 osdViewer hidden"></div>
   <div id="osd-viewer-2" class="container-fluid h-100 w-100 p-0 osdViewer hidden"></div>

   **<div id ="nubbin" class="nubbin"></div>**

...
...


## findme todo:  
Rewrite Readme
Clean code
upload demo
##----------------------------------------------------------------------------------------------------------------------------------------
