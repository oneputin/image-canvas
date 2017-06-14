# canvas based image-modifications
the elements containing a "canvas" used for rotation modifications of the raw image (must?) be "hidden" 
by *styling* it outside the viewport   
```` css
:host {
    display: inline-block;
    overflow: hidden;
    position: relative;
    left: -1000px;
}
````

the result (dataUrl) can then be "copied" into `visible` image-containers 

## The interactive canvas 
contains 2 canvas 
- first: downsizing the primary img to a copy fitting the actual device measures
- second: manipulating  

To run "interactive" modifications the original img must be copied into another canvas with gui-friendly size   



## resize-image
resizes an img-src (url, dataUrl) to another dataUrl. 
Based on `canvas`-resizing see (Tom Trenka on August 6, 2013)[https://davidwalsh.name/resize-image-canvas] 

resize-parameters:
+ height [px]
+ quality [0..1]
+ img-format (jpeg, png, ...)

## rotate-image
rotate parameters:
+ degreest [°]
+ quality [0..1]
+ img-format (jpeg, png, ...)
 


### demo-db

### demo-drop



## resize-percent
resizes an img-src (url, dataUrl) to another dataUrl. 

resize-parameters:
+ percent size of original [%]
+ guide-size [kB]
+ img-format (jpeg, png, ...)

### demo-drop-percent


### demo-batch




