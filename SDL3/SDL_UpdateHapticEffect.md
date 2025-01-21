###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_UpdateHapticEffect

Update the properties of an effect.

## Header File

Defined in [<SDL3/SDL_haptic.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_haptic.h)

## Syntax

```c
bool SDL_UpdateHapticEffect(SDL_Haptic *haptic, int effect, const SDL_HapticEffect *data);
```

## Function Parameters

|                                              |            |                                                                                                |
| -------------------------------------------- | ---------- | ---------------------------------------------------------------------------------------------- |
| [SDL_Haptic](SDL_Haptic) *                   | **haptic** | the [SDL_Haptic](SDL_Haptic) device that has the effect.                                       |
| int                                          | **effect** | the identifier of the effect to update.                                                        |
| const [SDL_HapticEffect](SDL_HapticEffect) * | **data**   | an [SDL_HapticEffect](SDL_HapticEffect) structure containing the new effect properties to use. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Can be used dynamically, although behavior when dynamically changing
direction may be strange. Specifically the effect may re-upload itself and
start playing from the start. You also cannot change the type either when
running [SDL_UpdateHapticEffect](SDL_UpdateHapticEffect)().

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_CreateHapticEffect](SDL_CreateHapticEffect)
- [SDL_RunHapticEffect](SDL_RunHapticEffect)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

