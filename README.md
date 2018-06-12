# ISF TouchDesigner

A TouchDesigner component parsing ISF-flavoured GLSL code into
TouchDesigner-flavoured GLSL. Uniform variables are exposes as
custom parameters.

This is not a full implementation of ISF features but it covers all basic features. About 90% of projects from https://interactiveshaderformat.com are
working correctly.

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
* The Python code could be refactored

## Maintenance

Issue reports and pull requests are welcome.
