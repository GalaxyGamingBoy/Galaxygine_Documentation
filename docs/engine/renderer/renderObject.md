# RenderObject

This file contains the RenderObject methods of Galaxygine, from the initalizing the RenderObject to rendering it.

## Methods

The methods avainable are:

-   [constructor(position, type): void](#constructorposition-type-void)
-   [getPosition(): Vector2](#getposition-vector2)
-   [getID(): string](#getid-string)
-   [getType(): string](#gettype-string)
-   [setPosition(newPosition): void](#setpositionnewposition-string)
-   [setID(newID): void](#setidnewid-string)
-   [render(context): void](#rendercontext-void)

### constructor(position, type): void

| Parameter | Parameter Type | Default        | Usage                            |
| --------- | -------------- | -------------- | -------------------------------- |
| position  | Vector2        | new Vector2()  | The position of the RenderObject |
| type      | string         | 'renderObject' | The type of the RenderObject     |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

The constructor of the RenderObject class.

### getPosition(): Vector2

| Parameter | Parameter Type | Default | Usage |
| --------- | -------------- | ------- | ----- |
| -         | -              | -       | -     |

| Return Value | Return Type | Usage                            |
| ------------ | ----------- | -------------------------------- |
| position     | Vector2     | The position of the RenderObject |

This function return the RenderObject's position.

### getID(): string

| Parameter | Parameter Type | Default | Usage |
| --------- | -------------- | ------- | ----- |
| -         | -              | -       | -     |

| Return Value | Return Type | Usage                      |
| ------------ | ----------- | -------------------------- |
| id           | string      | The id of the RenderObject |

This function return the RenderObject's id.

### getType(): string

| Parameter | Parameter Type | Default | Usage |
| --------- | -------------- | ------- | ----- |
| -         | -              | -       | -     |

| Return Value | Return Type | Usage                        |
| ------------ | ----------- | ---------------------------- |
| type         | string      | The type of the RenderObject |

This function return the RenderObject's type.

### setPosition(newPosition): string

| Parameter   | Parameter Type | Default       | Usage                                 |
| ----------- | -------------- | ------------- | ------------------------------------- |
| newPosition | Vector2        | new Vector2() | The new position of this RenderObject |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

This function sets the RenderObject's position.

### setID(newID): string

| Parameter | Parameter Type | Default | Usage                           |
| --------- | -------------- | ------- | ------------------------------- |
| newID     | string         | ' '     | The new id of this RenderObject |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

This function sets the RenderObject's id.

### render(context): void

| Parameter | Parameter Type           | Default | Usage                                                 |
| --------- | ------------------------ | ------- | ----------------------------------------------------- |
| context   | CanvasRenderingContext2D | -       | The context that the RenderObject will be rendered in |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

This function renders the RenderObject.