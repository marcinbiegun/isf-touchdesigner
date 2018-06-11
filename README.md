# ISF TouchDesigner

A TouchDesigner OP understanding ISF shaders. The workflow is fully
automated, with one click you get a working shader with exposed
controls.

![Screenshot](https://raw.githubusercontent.com/marcinbiegun/isf-touchdesigner/master/docs/screenshot.png)

## Features

* Float, color, long (list), bool, shape types are supported. This covers >90% of examples found at https://interactiveshaderformat.com
* ISF controls are set as Custom Parameters
* Image / video input
* Custom resolution
* Works with latest TouchDesigner 099
* GLSL code translation is wrritten in a single Python script, it's
  rather easy to follow

## What's missing?

* Multiple shader passes and a few built-in methods are missing
* The Python code could be refactored

## Maintenance

Issue reports and pull requests are welcome.
