# ISF TouchDesigner

ISF is a format that contains GLSL pixel shader and metadata on how users can
interact with uniform variables as sliders, buttons, etc. Big kudos
for [Vidvox](http://vidvox.net/) for creating it!

This is a TouchDesigner component parsing ISF-flavoured GLSL code into
TouchDesigner-flavoured GLSL. Uniform variables are exposes as
custom parameters.

This is not a full implementation of ISF features but it covers all basic features. Most compositions (using a single shader pass) from https://interactiveshaderformat.com are working correctly.

![Screenshot](https://raw.githubusercontent.com/marcinbiegun/isf-touchdesigner/master/docs/screenshot.png)

## Features

* Float, color, long (list), bool and shape ISF types are supported
* ISF controls are exposed as custom oarameters
* Image / video input
* Custom resolution
* GLSL code translation is done by a single Python script, it's
  rather easy to follow
* Works with latest TouchDesigner 099

## What's missing?

* Multiple shader passes
* A few less popular built-in methods

## Maintenance

Issue reports and pull requests are welcome.
