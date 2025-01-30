###### (This function is part of SDL_net, a separate library from SDL.)
# SDLNet_LinkedVersion

Query the verion of the SDL_net library in use at runtime.

## Header File

Defined in [<SDL3_net/SDL_net.h>](https://github.com/libsdl-org/SDL_net/blob/main/include/SDL3_net/SDL_net.h)

## Syntax

```c
const SDL_Version * SDLNet_LinkedVersion(void);

```

## Return Value

Returns An object with the runtime library version. Never returns NULL.

## Remarks

The returned value points to static, internal, read-only memory. Do not
modify or free it. The pointer remains valid as long as the library is
loaded by the system.

This function can be safely called before [SDLNet_Init](SDLNet_Init)().

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL_Net 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction)

