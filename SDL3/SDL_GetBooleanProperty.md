# SDL_GetBooleanProperty

Get a boolean property from a group of properties.

## Header File

Defined in [<SDL3/SDL_properties.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_properties.h)

## Syntax

```c
bool SDL_GetBooleanProperty(SDL_PropertiesID props, const char *name, bool default_value);
```

## Function Parameters

|                                      |                   |                                    |
| ------------------------------------ | ----------------- | ---------------------------------- |
| [SDL_PropertiesID](SDL_PropertiesID) | **props**         | the properties to query.           |
| const char *                         | **name**          | the name of the property to query. |
| bool                                 | **default_value** | the default value of the property. |

## Return Value

(bool) Returns the value of the property, or `default_value` if it is not
set or not a boolean property.

## Remarks

You can use [SDL_GetPropertyType](SDL_GetPropertyType)() to query whether
the property exists and is a boolean property.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetPropertyType](SDL_GetPropertyType)
- [SDL_HasProperty](SDL_HasProperty)
- [SDL_SetBooleanProperty](SDL_SetBooleanProperty)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryProperties](CategoryProperties)

