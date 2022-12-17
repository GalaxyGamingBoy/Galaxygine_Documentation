# Galaxygine

This file contains the methods of Galaxygine.

## Methods

The methods avainable are:

-   [setCanvasContext(context): void](#setcanvascontextcontext-void)
-   [galaxygineMainLoop(customCode): void](#galaxyginemainloopcustomcode-void)

### setCanvasContext(context): void

| Parameter | Parameter Type           | Default | Usage                                               |
| --------- | ------------------------ | ------- | --------------------------------------------------- |
| context   | CanvasRenderingContext2D | -       | The new context that will be assigned to Galaxygine |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

Sets all the canvas context that are needed for Galaxygine.  
i.e. The Draw class
!!! note
    This method is intended to be used with the `Core.engineInitialization` as its parameter

### galaxygineMainLoop(customCode): void

| Parameter  | Parameter Type | Default | Usage                                                              |
| ---------- | -------------- | ------- | ------------------------------------------------------------------ |
| customCode | Function       | -       | The function that will be executed every [tick](../utils/settings) |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

The main loop of Galaxygine that will be run every [tick](../engine/utils/settings.md)
!!! warning
    Erasing and Redrawing the Canvas are already there.  
    There is no need to add them to your customCode function.
!!! note
    A callback is expected, even an empty one.