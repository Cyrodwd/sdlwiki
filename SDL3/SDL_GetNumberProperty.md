###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetNumberProperty

Get a number property from a group of properties.

## Header File

Defined in [<SDL3/SDL_properties.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_properties.h)

## Syntax

```c
Sint64 SDL_GetNumberProperty(SDL_PropertiesID props, const char *name, Sint64 default_value);
```

## Function Parameters

|                                      |                   |                                    |
| ------------------------------------ | ----------------- | ---------------------------------- |
| [SDL_PropertiesID](SDL_PropertiesID) | **props**         | the properties to query.           |
| const char *                         | **name**          | the name of the property to query. |
| [Sint64](Sint64)                     | **default_value** | the default value of the property. |

## Return Value

([Sint64](Sint64)) Returns the value of the property, or `default_value` if
it is not set or not a number property.

## Remarks

You can use [SDL_GetPropertyType](SDL_GetPropertyType)() to query whether
the property exists and is a number property.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetPropertyType](SDL_GetPropertyType)
- [SDL_HasProperty](SDL_HasProperty)
- [SDL_SetNumberProperty](SDL_SetNumberProperty)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryProperties](CategoryProperties)

