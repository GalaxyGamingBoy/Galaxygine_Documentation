# InputHandler

This file contains the InputHandler methods of Galaxygine, from detecting keypresses to detecting key actions.

## Methods

The methods avainable are:

-   getKeyPressArray(): Array<string>
-   isKeyPressed(key): boolean
-   isAnyKeyPressed(): boolean
-   isKeyArrayPressed(keyArray): boolean
-   isKeyActionPressed(actionID): boolean

### getKeyPressArray(): Array<string>

| Parameter | Parameter Type | Default | Usage |
| --------- | -------------- | ------- | ----- |
| -         | -              | -       | -     |

| Return Value | Return Type   | Usage                                             |
| ------------ | ------------- | ------------------------------------------------- |
| keyArray     | Array<string> | An array containing all the keys that are pressed |

This function returns an array containg all the keys that are currently pressed.

### isKeyPressed(key): boolean

| Parameter | Parameter Type | Default | Usage                |
| --------- | -------------- | ------- | -------------------- |
| key       | string         | ' '     | The keyCode to check |

| Return Value | Return Type | Usage                          |
| ------------ | ----------- | ------------------------------ |
| isKeyPressed | boolean     | Is this key currently pressed? |

This function returns a boolean with the value indicating if the key is pressed.

### isAnyKeyPressed(): boolean

| Parameter | Parameter Type | Default | Usage |
| --------- | -------------- | ------- | ----- |
| -         | -              | -       | -     |

| Return Value    | Return Type | Usage               |
| --------------- | ----------- | ------------------- |
| isAnyKeyPressed | boolean     | Is any key pressed? |

This function returns a boolean with the value indicating if the any key is pressed.

### isKeyArrayPressed(keyArray): boolean

| Parameter | Parameter Type | Default | Usage                               |
| --------- | -------------- | ------- | ----------------------------------- |
| keyArray  | Array<string>  | []      | An array with the keyCodes to check |

| Return Value              | Return Type | Usage               |
| ------------------------- | ----------- | ------------------- |
| isAnyKeyInKeyArrayPressed | boolean     | Is any key pressed? |

This function returns a boolean with the value indicating if the any key in the keyArray is pressed.

### isKeyActionPressed(actionID): boolean

| Parameter | Parameter Type | Default | Usage                               |
| --------- | -------------- | ------- | ----------------------------------- |
| keyArray  | Array<string>  | []      | An array with the keyCodes to check |

| Parameter | Parameter Type | Default | Usage                         |
| --------- | -------------- | ------- | ----------------------------- |
| actionID  | string         | ' '     | The id of the action to check |

This function returns a boolean with the value indicating if a key in the keyAction with the specified actionID is pressed.

!!! note
    For more info on keyActions click [here](../../res/keyAction.md)