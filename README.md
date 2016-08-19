# \<resize-image\>

resize an image and output as base64 

## Source
derived from article by (Dr. Tom Trenka on August 6, 2013)[https://davidwalsh.name/resize-image-canvas]

## Divided 
into 2 elements:
+ drop-zone processing `file.drop`
+ image-resizing `resize-image` 

# Interactive Demos: 
## Drop and Resize 
`drop-demo.html` as demo of `file-drop.html` 

## Resizing a set of images managed in Firebase-DB   
`resize-demo.html` as demo of `resize-image.html`

to create a minified dataurl for every image in a dataset requested from wolken-db which can be used as `preload-image` in `iron-image`, z.B. in catalog-viewer.

## Batch resize from firebase
`resize-all.html` and `resize-all-check.html` : 

Open question: How to detect the end of the primary (async) resize-batch  after <template is="dom-repeat" items="[[clientitems]]"> -- ??? may be better better per script with promises ???  


## ALERT
Because the `canvas.toDataURL()` does not work with CORS-"tainted" canvas 
- the images must be transfered into the same domain (fi. into localhost as here)  or
- the images folder at its server must be CORS-enabled for the requesting site !!

## 

