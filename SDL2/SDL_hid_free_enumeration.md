# SDL_hid_free_enumeration

Free an enumeration Linked List

## Header File

Defined in [SDL_hidapi.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hidapi.h)

## Syntax

```c
void SDL_hid_free_enumeration(SDL_hid_device_info *devs);
```

## Function Parameters

|                                              |          |                                                                                            |
| -------------------------------------------- | -------- | ------------------------------------------------------------------------------------------ |
| [SDL_hid_device_info](SDL_hid_device_info) * | **devs** | Pointer to a list of struct_device returned from [SDL_hid_enumerate](SDL_hid_enumerate)(). |

## Remarks

This function frees a linked list created by
[SDL_hid_enumerate](SDL_hid_enumerate)().

## Version

This function is available since SDL 2.0.18.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHIDAPI](CategoryHIDAPI)

