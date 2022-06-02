# ISF TouchDesigner

ISF is a format that contains GLSL pixel shader and metadata on how users can
interact with uniform variables as sliders, buttons, etc. Big kudos
for [Vidvox](http://vidvox.net/) for creating it!

This component parses ISF-flavoured GLSL code into
TouchDesigner-flavoured GLSL.

The workflow is very simple - just connect a Text DAT with ISF source code, it will work and expose defined input variables as custom parameters on the OP.

This is not a full implementation of ISF but it covers most commonly used features. About 80% of compositions from https://interactiveshaderformat.com are working correctly.

![Screenshot](https://raw.githubusercontent.com/marcinbiegun/isf-touchdesigner/master/docs/screenshot.png)

## Shader code compatibility

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
IMG_NORM_PIXEL()
IMG_SIZE()
```

## Features

* Input types: `float`, `color`, `long`, `bool`, `event`, `shape`
* ISF controls are exposed as custom parameters on Base OP
* Image / video input
* Custom resolution
* GLSL code translation is done by a single Python script, it's
  rather easy to follow
* Works with latest TouchDesigner 099
* Multiple passes (1 and 2)

## What's missing

* Third pass
* Vertex shader

## Changelog

### 2022.06.02

* fixed compatibility with TouchDesigner 2020.24200
* added support for TIMEDELTA keyword

### 2020.05.28

* fixed compatibility with TouchDesigner 2020
* float parameters exposed as relative value in 0.0 to 1.0 range
  instead of absolute value

### 2018.06.13

* initial release

## Contribuing

Issue reports and pull requests are welcome.
