# Key Actions
Key Actions are contained in a json file named `keyActions.json` on the `src/res/` folder of the project.

## Usage
Key Actions are used to detect any key press on a group of keys.  
Each key action has a different actionID that makes the action unique.

### Example
You need to move a 2D character left or right but with each action has more than one key.  

**Without** key actions you would do:
```typescript title="index.ts"
import { Galaxygine } from './Galaxygine';

const galaxygine = new Galaxygine();
galaxygine.setCanvasContext(galaxygine.Core.engineInitialization());

galaxygine.galaxygineMainLoop(() => {
     if (galaxygine.InputHandler.isKeyPressed("d") || galaxygine.InputHandler.isKeyPressed("ArrowRight")) {
        console.log("MoveRight")
     }
});
```

**With** key actions you would do:
```json title="keyActions.json"
[
    {
        "actionID": "key_right",
        "keys": [
            "d",
            "ArrowRight"
        ]
    }
]
```

```typescript title="index.ts"
import { Galaxygine } from './Galaxygine';

const galaxygine = new Galaxygine();
galaxygine.setCanvasContext(galaxygine.Core.engineInitialization());

galaxygine.galaxygineMainLoop(() => {
     if (galaxygine.InputHandler.isKeyActionPressed("key_right")) {
        console.log("MoveRight")
     }
});
```

## File Template
Below is a template of keyActions.json
```json title="src/res/keyActions.json"
[
    {
        "actionID": "key_right",
        "keys": [
            "d",
            "ArrowRight"
        ]
    },
    {
        "actionID": "key_left",
        "keys": [
            "a",
            "ArrowLeft"
        ]
    }
]
```