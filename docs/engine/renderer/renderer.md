# Renderer

This file contains the Renderer methods of Galaxygine, from rendering objects to getting RenderObjects.

## Terminology
`RenderObject`: A render object is a class with logic for rendering it.  
`Object`: An object is an array of the `RenderObject` and it's `id`. Syntax: `[ RenderObject, id ]`

## Methods

The methods avainable are:

-   [getRenderObject(index): [RenderObject, number]](#getrenderobjectindex-renderobject-number)
-   [getRenderObjectByID(id): [RenderObject. number] | number](#getrenderobjectbyidid-renderobject-number-number)
-   [setRenderObject(object): void](#setrenderobjectobject-void)
-   [setRenderObjectByID(id, renderObject): void](#setrenderobjectbyidid-renderobject-void)
-   [addRenderObject(renderObject): void](#addrenderobjectrenderobject-void)
-   [renderObjects(context): void](#renderobjectscontext-void)

### getRenderObject(index): [RenderObject, number]

| Parameter | Parameter Type | Default | Usage                          |
| --------- | -------------- | ------- | ------------------------------ |
| index     | number         | 0       | The index of the object to get |

| Return Value | Return Type            | Usage               |
| ------------ | ---------------------- | ------------------- |
| object       | [RenderObject, number] | The returned object |

Gets a object with the specified index.

### getRenderObjectByID(id): [RenderObject, number] | number

| Parameter | Parameter Type | Default | Usage                       |
| --------- | -------------- | ------- | --------------------------- |
| id        | string         | ' '     | The id of the object to get |

| Return Value | Return Type            | Usage                                     |
| ------------ | ---------------------- | ----------------------------------------- |
| object       | [RenderObject, number] | The returned object **if** an id is found |
| errorCode    | number                 | The error code **if an error occurred**   |

!!! note
    If an object with the id isn't found, it count's as an error
Gets a object with the specified id.

### setRenderObject(object): void

| Parameter | Parameter Type         | Default                 | Usage             |
| --------- | ---------------------- | ----------------------- | ----------------- |
| object    | [RenderObject, number] | [new RenderObject(), 0] | The object to set |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

Sets a render object at the specified index.

### setRenderObjectByID(id, renderObject): void

| Parameter    | Parameter Type | Default            | Usage                    |
| ------------ | -------------- | ------------------ | ------------------------ |
| id           | string         | ' '                | The id to set            |
| renderObject | RenderObject   | new RenderObject() | The render object to set |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

Sets a render object at the specified id.

### addRenderObject(renderObject): void

| Parameter    | Parameter Type | Default            | Usage                    |
| ------------ | -------------- | ------------------ | ------------------------ |
| renderObject | RenderObject   | new RenderObject() | The render object to set |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

Adds a render object at the last index of the render path.

### renderObjects(context): void

| Parameter | Parameter Type           | Default | Usage                           |
| --------- | ------------------------ | ------- | ------------------------------- |
| context   | CanvasRenderingContext2D | -       | The 2D canvas rendering context |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

Renders all objects on the renderPath.