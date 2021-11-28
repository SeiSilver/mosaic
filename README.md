**Config**

```
TILE_SIZE      = 200	# height/width of mosaic tiles in pixels
TILE_MATCH_RES = 3		# tile matching resolution (higher values give better fit but require more processing)
ENLARGEMENT    = 4		# the mosaic image will be this many times wider and taller than the original
```

**Install Pillow & numpy**

```
python3 -m pip install --upgrade pip
python3 -m pip install --upgrade Pillow
python3 -m pip install numpy
```

**How to Run**

```
python ./scripts/mosaic.py [location-of-image-want-to-created] [location-of-sub-images]
```

**Example**

```
python ./scripts/mosaic.py ./data/origin.jpg ./data/hololive
```

**Large Image Fix**

```
# we will set the MAX_IMAGE_PIXELS to none to remove the image size limited (not recommended)
Image.MAX_IMAGE_PIXELS = None
```