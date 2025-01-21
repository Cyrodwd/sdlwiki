###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_hid_get_product_string

Get The Product String from a HID device.

## Header File

Defined in [<SDL3/SDL_hidapi.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_hidapi.h)

## Syntax

```c
int SDL_hid_get_product_string(SDL_hid_device *dev, wchar_t *string, size_t maxlen);
```

## Function Parameters

|                                    |            |                                                               |
| ---------------------------------- | ---------- | ------------------------------------------------------------- |
| [SDL_hid_device](SDL_hid_device) * | **dev**    | a device handle returned from [SDL_hid_open](SDL_hid_open)(). |
| wchar_t *                          | **string** | a wide string buffer to put the data into.                    |
| size_t                             | **maxlen** | the length of the buffer in multiples of wchar_t.             |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHIDAPI](CategoryHIDAPI)

