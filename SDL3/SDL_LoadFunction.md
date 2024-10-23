###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_LoadFunction

Look up the address of the named function in a shared object.

## Header File

Defined in [<SDL3/SDL_loadso.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_loadso.h)

## Syntax

```c
SDL_FunctionPointer SDL_LoadFunction(SDL_SharedObject *handle, const char *name);
```

## Function Parameters

|                                        |            |                                                                              |
| -------------------------------------- | ---------- | ---------------------------------------------------------------------------- |
| [SDL_SharedObject](SDL_SharedObject) * | **handle** | a valid shared object handle returned by [SDL_LoadObject](SDL_LoadObject)(). |
| const char *                           | **name**   | the name of the function to look up.                                         |

## Return Value

([SDL_FunctionPointer](SDL_FunctionPointer)) Returns a pointer to the
function or NULL on failure; call [SDL_GetError](SDL_GetError)() for more
information.

## Remarks

This function pointer is no longer valid after calling
[SDL_UnloadObject](SDL_UnloadObject)().

This function can only look up C function names. Other languages may have
name mangling and intrinsic language support that varies from compiler to
compiler.

Make sure you declare your function pointers with the same calling
convention as the actual library function. Your code will crash
mysteriously if you do not do this.

If the requested function doesn't exist, NULL is returned.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.1.3.

## Code Examples

```c

/* Variable declaration */
SDL_SharedObject* myHandle = NULL;
const char* myFunctionName = "myFancyFunction";
void (*myFancyFunction)(int anInt);

/* Dynamically load mylib.so */
myHandle = SDL_LoadObject("mylib.so");

/* Load the exported function from mylib.so
 * The exported function has the following prototype
 * void myFancyFunction(int anInt);
 */
myFancyFunction = (void (*)(int))SDL_LoadFunction(myHandle, myFunctionName);

/* Call myFancyFunction with a random integer */
if (myFancyFunction != NULL) {
    myFancyFunction(15);
} else {
    /* Error handling here */
}
```

## See Also

- [SDL_LoadObject](SDL_LoadObject)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySharedObject](CategorySharedObject)

