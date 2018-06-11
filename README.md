# ISF TouchDesigner

A TouchDesigner component parsing ISF-flavoured GLSL code into
TouchDesigner-flavoured GLSL and connecting uniforms to exposed
TouchDesigner customer parameters.

About 90% of examples found at https://interactiveshaderformat.com are
working correctly.

![Screenshot](https://raw.githubusercontent.com/marcinbiegun/isf-touchdesigner/master/docs/screenshot.png)

## Features

* Float, color, long, bool, shape ISF types are supported
* ISF controls are exposed as Custom Parameters
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
