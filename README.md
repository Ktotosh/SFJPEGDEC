# SFJPEGDEC

## Overview
This is a baseline JPEG decoder made in starfall/wire for gmod. It uses a wiremod digital screen instead of a starfall screen so you must also have wiremod installed.

## Usage
It supports a vaiety of different JPEGs but it does not support:
- Progressive jpegs (will cause a huffman table error)
- RGB jpegs
- Any other type of jpeg that isnt YCbCr
- Any jpeg which has more than 786432 pixels (a limitation of the wire digital screen)

The file path is relative to the game folder (eg. steamapps/common/GarrysMod/garrysmod)
OpsLimit defines the max processor time in ms. I recommend setting this to 1-4
Spawn a digital screen first and then place the chip on it. It will automatically configure the screen settings for the image
Also set sf_net_burstmax_cl and sf_net_burstrate_cl to something high so the chip won't throw an error.

## Screenshots
Basic JPG decoding
![Example](https://raw.githubusercontent.com/Ktotosh/SFJPEGDEC/refs/heads/main/screenshots/20260713171421_1.jpg)
