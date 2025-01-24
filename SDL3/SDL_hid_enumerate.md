# SDL_hid_enumerate

Enumerate the HID Devices.

## Header File

Defined in [<SDL3/SDL_hidapi.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_hidapi.h)

## Syntax

```c
SDL_hid_device_info * SDL_hid_enumerate(unsigned short vendor_id, unsigned short product_id);
```

## Function Parameters

|                |                |                                                                                 |
| -------------- | -------------- | ------------------------------------------------------------------------------- |
| unsigned short | **vendor_id**  | the Vendor ID (VID) of the types of device to open, or 0 to match any vendor.   |
| unsigned short | **product_id** | the Product ID (PID) of the types of device to open, or 0 to match any product. |

## Return Value

([SDL_hid_device_info](SDL_hid_device_info) *) Returns a pointer to a
linked list of type [SDL_hid_device_info](SDL_hid_device_info), containing
information about the HID devices attached to the system, or NULL in the
case of failure. Free this linked list by calling
[SDL_hid_free_enumeration](SDL_hid_free_enumeration)().

## Remarks

This function returns a linked list of all the HID devices attached to the
system which match vendor_id and product_id. If `vendor_id` is set to 0
then any vendor matches. If `product_id` is set to 0 then any product
matches. If `vendor_id` and `product_id` are both set to 0, then all HID
devices will be returned.

By default SDL will only enumerate controllers, to reduce risk of hanging
or crashing on bad drivers, but
[SDL_HINT_HIDAPI_ENUMERATE_ONLY_CONTROLLERS](SDL_HINT_HIDAPI_ENUMERATE_ONLY_CONTROLLERS)
can be set to "0" to enumerate all HID devices.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_hid_device_change_count](SDL_hid_device_change_count)


## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHIDAPI](CategoryHIDAPI)

