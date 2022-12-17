# Sound

This file contains the Sound methods of Galaxygine, from loading sounds to playing them.

## Methods

The methods avainable are:

-   [addSound(soundID, soundPath): void](#addsoundsoundid-soundpath-void)
-   [removeSound(soundID): void](#removesoundsoundid-void)
-   [removeALLSounds(): void](#removeallsound-void)
-   [getSoundLibrary(): Array<{soundID: string; sound: HTMLAudioElement}>](#getsoundlibrary-arraysoundid-string-sound-htmlaudioelement)
-   [getSoundElementFromLibrary(soundID): number | {soundID: string; sound: HTMLAudioElement}](#getsoundelementfromlibrarysoundid-number-soundid-string-sound-htmlaudioelement)
-   [playSound(soundID): void](#playsoundsoundid-void)
-   [stopSound(soundID): void](#stopsoundsoundid-void)

### addSound(soundID, soundPath): void

| Parameter | Parameter Type | Default | Usage                                     |
| --------- | -------------- | ------- | ----------------------------------------- |
| soundID   | string         | ' '     | The id that will be assigned on the sound |
| soundPath | string         | ' '     | The location of the sound                 |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

This function adds a sound to the sound library.

### removeSound(soundID): void

| Parameter | Parameter Type | Default | Usage                                     |
| --------- | -------------- | ------- | ----------------------------------------- |
| soundID   | string         | ' '     | The id that will be assigned on the sound |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

This function removes a sound from the sound library.

### removeALLSound(): void

| Parameter | Parameter Type | Default | Usage |
| --------- | -------------- | ------- | ----- |
| -         | -              | -       | -     |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

This function removes all sounds from the sound library.

### getSoundLibrary(): Array<{soundID: string; sound: HTMLAudioElement}>

| Parameter | Parameter Type | Default | Usage |
| --------- | -------------- | ------- | ----- |
| -         | -              | -       | -     |

| Return Value | Return Type                                       | Usage                     |
| ------------ | ------------------------------------------------- | ------------------------- |
| soundLibrary | Array<{soundID: string; sound: HTMLAudioElement}> | The current sound library |

This function returns the the sound library.

### getSoundElementFromLibrary(soundID): number | {soundID: string; sound: HTMLAudioElement}

| Parameter | Parameter Type | Default | Usage                      |
| --------- | -------------- | ------- | -------------------------- |
| soundID   | string         | ' '     | The id of the sound to get |

| Return Value | Return Type                                | Usage                                        |
| ------------ | ------------------------------------------ | -------------------------------------------- |
| sound        | {soundID: string; sound: HTMLAudioElement} | The sound to be returned **if** it is found. |
| errorCode    | number                                     | Returns -1 **if it is not** found            |

This function returns a sound with the specified soundID from the current sound library.

### playSound(soundID): void

| Parameter | Parameter Type | Default | Usage                      |
| --------- | -------------- | ------- | -------------------------- |
| soundID   | string         | ' '     | The id of the sound to get |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

This function plays a sound with the specified soundID.

### stopSound(soundID): void

| Parameter | Parameter Type | Default | Usage                      |
| --------- | -------------- | ------- | -------------------------- |
| soundID   | string         | ' '     | The id of the sound to get |

| Return Value | Return Type | Usage |
| ------------ | ----------- | ----- |
| -            | -           | -     |

This function stops a sound with the specified soundID.