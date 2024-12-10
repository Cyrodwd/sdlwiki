###### (This function is part of SDL_image, a separate library from SDL.)
# IMG_SaveJPG

Save an SDL_Surface into a JPEG image file.

## Header File

Defined in [<SDL3_image/SDL_image.h>](https://github.com/libsdl-org/SDL_image/blob/main/include/SDL3_image/SDL_image.h)

## Syntax

```c
bool IMG_SaveJPG(SDL_Surface *surface, const char *file, int quality);
```

## Function Parameters

|               |             |                                                                                      |
| ------------- | ----------- | ------------------------------------------------------------------------------------ |
| SDL_Surface * | **surface** | the SDL surface to save.                                                             |
| const char *  | **file**    | path on the filesystem to write new file to.                                         |
| int           | **quality** | [0; 33] is Lowest quality, [34; 66] is Middle quality, [67; 100] is Highest quality. |

## Return Value

(bool) Returns true on success or false on failure; call SDL_GetError() for
more information.

## Remarks

If the file already exists, it will be overwritten.

## Version

This function is available since SDL_image 3.0.0.

## See Also

- [IMG_SaveJPG_IO](IMG_SaveJPG_IO)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLImage](CategorySDLImage)

