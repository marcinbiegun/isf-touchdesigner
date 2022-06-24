# ISF TouchDesigner

This component integrates ISF shaders into TouchDesigner.

Discussion thread: [https://forum.derivative.ca/t/isf-parser/10588](https://forum.derivative.ca/t/isf-parser/10588)

## What is ISF?

ISF (Interactive Sahder Format) is wrapper around GLSL pixel shaders. It standarizes way
to create live video effects that can be then used in and controlled by VJ Software.

Learn more about ISF here: [https://isf.video/](https://isf.video/)

## How to use it

The workflow is very simple:

1. Create a Text DAT node, paste some ISF code there and connect it to isfParser component.
2. Connect your video input to the component.
3. Click "Reload" and it's done! You will receive the video output and you can play with the ISF parameters that will be now visible on the component.

![Screenshot](https://raw.githubusercontent.com/marcinbiegun/isf-touchdesigner/master/docs/screenshot.png)

## Compatibility

Supported variables:

```
PASSINDEX
RENDERSIZE
isf_FragNormCoord
TIME
TIMEDELTA
DATE
FRAMEINDEX
```

Supported functions:

```
IMG_PIXEL()
IMG_THIS_PIXEL()
IMG_NORM_PIXEL()
IMG_THIS_NORM_PIXEL()
IMG_SIZE()
```

Supported input types:

```
float
color
long
bool
event
shape
```

## Features

* ISF controls are exposed as custom parameters on Base OP
* Image / video input
* Custom resolution
* GLSL code translation is done by a single Python script, it's
  rather easy to follow
* Works with latest TouchDesigner
* Multiple passes (1 and 2)

## What's missing

* Third pass
* Vertex shader

## Changelog

### 2022.06.24

* fix `IMG_THIS_PIXEL` and `IMG_THIS_NORM_PIXEL` sampler functions

### 2022.06.02

* fixed compatibility with TouchDesigner 2022.24200
* added support for TIMEDELTA keyword

### 2020.05.28

* fixed compatibility with TouchDesigner 2020
* float parameters exposed as relative value in 0.0 to 1.0 range
  instead of absolute value

### 2018.06.13

* initial release

## Contribuing

Issue reports and pull requests are welcome.
