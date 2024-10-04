###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_hid_get_indexed_string

Get a string from a HID device, based on its string index.

## Header File

Defined in [SDL_hidapi.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hidapi.h)

## Syntax

```c
int SDL_hid_get_indexed_string(SDL_hid_device *dev, int string_index, wchar_t *string, size_t maxlen);
```

## Function Parameters

|                                    |                  |                                                               |
| ---------------------------------- | ---------------- | ------------------------------------------------------------- |
| [SDL_hid_device](SDL_hid_device) * | **dev**          | A device handle returned from [SDL_hid_open](SDL_hid_open)(). |
| int                                | **string_index** | The index of the string to get.                               |
| wchar_t *                          | **string**       | A wide string buffer to put the data into.                    |
| size_t                             | **maxlen**       | The length of the buffer in multiples of wchar_t.             |

## Return Value

(int) Returns 0 on success and -1 on error.

## Version

This function is available since SDL 2.0.18.

## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHIDAPI](CategoryHIDAPI)

