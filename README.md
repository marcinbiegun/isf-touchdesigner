# ISF TouchDesigner

ISF is a format that contains GLSL pixel shader and metadata on how users can
interact with uniform variables as sliders, buttons, etc. Big kudos
for [Vidvox](http://vidvox.net/) for creating it!

This is a TouchDesigner component parsing ISF-flavoured GLSL code into
TouchDesigner-flavoured GLSL. Uniform variables are exposes as
custom parameters.

This is not a full implementation of ISF but it covers most commonly used features. About 80% of compositions from https://interactiveshaderformat.com are working correctly.

![Screenshot](https://raw.githubusercontent.com/marcinbiegun/isf-touchdesigner/master/docs/screenshot.png)

## Features

* Input types: float, color, long (list), bool, event, shape
* ISF controls are exposed as custom parameters on Base OP
* Image / video input
* Custom resolution
* GLSL code translation is done by a single Python script, it's
  rather easy to follow
* Works with latest TouchDesigner 099
* Multiple passes (only one)

## What's missing

* More than 1 additional pass
* Vertex shader
* A few less popular built-in methods

## Maintenance

Issue reports and pull requests are welcome.
