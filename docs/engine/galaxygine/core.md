# Core

This file contains core methods of Galaxygine, from the initialization to touchscreen checking.

## Methods

The methods avainable are:

-   [engineInitialization(mountID, canvasWidth, canvasHeight): CanvasRenderingContext2D](#engineinitializationmountid-canvaswidth-canvasheight-canvasrenderingcontext2d)
-   [getScreenSize(): Vector2](#getscreensize-vector2)
-   [hasTouchscreen(): Boolean](#hastouchscreen-boolean)

### engineInitialization(mountID, canvasWidth, canvasHeight): CanvasRenderingContext2D

| Parameter    | Parameter Type | Default            | Usage                                                               |
| ------------ | -------------- | ------------------ | ------------------------------------------------------------------- |
| mountID      | string         | galaxygine         | The id of the element that the Galaxygine canvas will be mounted on |
| canvasWidth  | number         | window.innerWidth  | The width of the canvas                                             |
| canvasHeight | number         | window.innerHeight | The height of the canvas                                            |

| Return Value       | Return Type              | Usage                                             |
| ------------------ | ------------------------ | ------------------------------------------------- |
| galaxygine_context | CanvasRenderingContext2D | The 2D canvas rendering context of the new canvas |

This function initializes Galaxygine by creating a canvas on the element with the id given to it by mountID and has a width of canvasWidth and height of canvasHeight.  

### getScreenSize(): Vector2

| Parameter | Parameter Type | Default | Usage |
|-----------|----------------|---------|-------|
| -         | -              | -       | -     |

| Return Value | Return Type | Usage                  |
|--------------|-------------|------------------------|
| windowSize   | Vector2     | The size of the window |

This function return the width and the height of the browser window.

### hasTouchscreen(): Boolean

| Parameter | Parameter Type | Default | Usage |
|-----------|----------------|---------|-------|
| -         | -              | -       | -     |

| Return Value     | Return Type | Usage                                        |
|------------------|-------------|----------------------------------------------|
| hasTouchscreen   | Boolean     | Does the device has a touchscreen connected? |

This function return a boolean indicating if the device has a touchscreen connected.