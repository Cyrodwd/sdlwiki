###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_hid_write

Write an Output report to a HID device.

## Header File

Defined in [<SDL3/SDL_hidapi.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_hidapi.h)

## Syntax

```c
int SDL_hid_write(SDL_hid_device *dev, const unsigned char *data, size_t length);
```

## Function Parameters

|                                    |            |                                                                  |
| ---------------------------------- | ---------- | ---------------------------------------------------------------- |
| [SDL_hid_device](SDL_hid_device) * | **dev**    | a device handle returned from [SDL_hid_open](SDL_hid_open)().    |
| const unsigned char *              | **data**   | the data to send, including the report number as the first byte. |
| size_t                             | **length** | the length in bytes of the data to send.                         |

## Return Value

(int) Returns the actual number of bytes written and -1 on on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

The first byte of `data` must contain the Report ID. For devices which only
support a single report, this must be set to 0x0. The remaining bytes
contain the report data. Since the Report ID is mandatory, calls to
[SDL_hid_write](SDL_hid_write)() will always contain one more byte than the
report contains. For example, if a hid report is 16 bytes long, 17 bytes
must be passed to [SDL_hid_write](SDL_hid_write)(), the Report ID (or 0x0,
for devices with a single report), followed by the report data (16 bytes).
In this example, the length passed in would be 17.

[SDL_hid_write](SDL_hid_write)() will send the data on the first OUT
endpoint, if one exists. If it does not, it will send the data through the
Control Endpoint (Endpoint 0).

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHIDAPI](CategoryHIDAPI)

