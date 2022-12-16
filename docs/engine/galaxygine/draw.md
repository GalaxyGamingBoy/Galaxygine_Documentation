# Draw

This file contains core methods of Galaxygine, from the initialization to touchscreen checking.

## Methods

The methods avainable are:

-	[constructor(context): void](#constructor-void)
-	[setCanvasContext(context): void](#setcanvascontext-void)
-	[drawRectangle(position, size, id, color): void](#drawrectangleposition-size-id-color-void)
-	[drawRectangleOutline(position, size, id, color): void](#drawrectangleoutlineposition-size-id-color-void)
-	[drawRectangleWithOutline(position, size, id, color): void](#drawrectanglewithoutlineposition-size-id-outlinecolor-squarecolor-void)
-	[drawImage(position, size, imagePath, id): void](#drawimageposition-size-imagepath-id-void)
-	[drawText(position, text, id, color, font): void](#drawtextposition-text-id-color-font-void)
-	[drawStrokeText(position, text, id, color, font): void](#drawstroketextposition-text-id-color-font-void)
-	[eraseRectangle(position, size): void](#eraserectangleposition-size-void)
-	[eraseCanvas(): void](#erasecanvas-void)

### constructor(): void

| Parameter | Parameter Type           | Default | Usage                                      |
| --------- | ------------------------ | ------- | ------------------------------------------ |
| context   | CanvasRenderingContext2D | -       | The context that will be used for graphics |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

Sets a renderer and the 2D context to use.

### setCanvasContext(): void

| Parameter | Parameter Type           | Default | Usage                                      |
| --------- | ------------------------ | ------- | ------------------------------------------ |
| context   | CanvasRenderingContext2D | -       | The context that will be used for graphics |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

Sets the 2D context to use.

### drawRectangle(position, size, id, color): void

| Parameter | Parameter Type | Default       | Usage                                               |
| --------- | -------------- | ------------- | --------------------------------------------------- |
| position  | Vector2        | Vector2(0, 0) | The position that the rectangle will be rendered in |
| size      | Vector2        | Vector2(0, 0) | The size that the rectangle will be                 |
| id        | string         | ' '           | The id that will be assigned on the rectangle       |
| color     | string         | '#000000'     | The color that the rectangle will be in             |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

Draws a rectange at the specified position with the specified size and the specified color.

### drawRectangleOutline(position, size, id, color): void

| Parameter | Parameter Type | Default       | Usage                                                              |
| --------- | -------------- | ------------- | ------------------------------------------------------------------ |
| position  | Vector2        | Vector2(0, 0) | The position that the outline of the rectangle will be rendered in |
| size      | Vector2        | Vector2(0, 0) | The size that the outline of the rectangle will be                 |
| id        | string         | ''            | The id that will be assigned on the outline of rectangle           |
| color     | string         | '#000000'     | The color that the outline of rectangle will be in                 |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

Draws an outline of a rectange at the specified position with the specified size and the specified color.

### drawRectangleWithOutline(position, size, id, outlineColor, squareColor): void

| Parameter      | Parameter Type | Default       | Usage                                               |
| -------------- | -------------- | ------------- | --------------------------------------------------- |
| position       | Vector2        | Vector2(0, 0) | The position that the rectangle will be rendered in |
| size           | Vector2        | Vector2(0, 0) | The size that the rectangle will be                 |
| id             | string         | ' '           | The id that will be assigned on the rectangle       |
| outlineColor   | string         | '#000000'     | The color that the outline of rectangle will be in  |
| rectangleColor | string         | '#000000'     | The color that the rectangle will be in             |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

Draws a rectange with a seperate outline at the specified position with the specified size and the specified color.  

!!! note
    The rectangle with the outline has an id of `id + '_outline'`.  
    i.e. If the id is `rect` the rectangle with the outline id will be `rect_outline`

### drawImage(position, size, imagePath, id): void

| Parameter | Parameter Type | Default       | Usage                                           |
| --------- | -------------- | ------------- | ----------------------------------------------- |
| position  | Vector2        | Vector2(0, 0) | The position that the image will be rendered in |
| size      | Vector2        | Vector2(0, 0) | The size that the image will be                 |
| imagePath | string         | ' '           | The file location of the image                  |
| id        | string         | ' '           | The id that will be assigned on the rectangle   |

Draws an image from the specified location in the specified position at the specified sized with the specified id

### drawText(position, text, id, color, font): void

| Parameter | Parameter Type | Default       | Usage                                           |
| --------- | -------------- | ------------- | ----------------------------------------------- |
| position  | Vector2        | Vector2(0, 0) | The position that the text will be rendered in  |
| text      | string         | ' '           | The text that will be shown                     |
| id        | string         | ' '           | The id that will be assigned on the rectangle   |
| color     | string         | '#000000'     | The color of the text                           |
| font      | string         | '48px serif'  | The font that the text will use to be displayed |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

Displays the specified text at the specified position with the specified id, color and font.

### drawStrokeText(position, text, id, color, font): void

| Parameter | Parameter Type | Default       | Usage                                                   |
| --------- | -------------- | ------------- | ------------------------------------------------------- |
| position  | Vector2        | Vector2(0, 0) | The position that the text will be rendered in          |
| text      | string         | ' '           | The text that will be shown                             |
| id        | string         | ' '           | The id that will be assigned on the rectangle           |
| color     | string         | '#000000'     | The color of the stroked text                           |
| font      | string         | '48px serif'  | The font that the stroked text will use to be displayed |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

Displays the specified stroked text at the specified position with the specified id, color and font.

### eraseRectangle(position, size): void

| Parameter | Parameter Type | Default       | Usage                                               |
| --------- | -------------- | ------------- | --------------------------------------------------- |
| position  | Vector2        | Vector2(0, 0) | The position that the rectangle will be rendered in |
| size      | Vector2        | Vector2(0, 0) | The size of the rectangle                           |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

Erases a rectangle on the specified position with the specifed size.

### eraseCanvas(): void

| Parameter | Parameter Type | Default | Usage |
| --------- | -------------- | ------- | ----- |
| -         | -              | -       | -     |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

Erases the whole canvas.