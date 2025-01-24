# SDL_HINT_GDK_TEXTINPUT_SCOPE

This variable sets the input scope of the TextInput window on GDK platforms.

## Header File

Defined in [<SDL3/SDL_hints.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_GDK_TEXTINPUT_SCOPE "SDL_GDK_TEXTINPUT_SCOPE"
```

## Remarks

Set this hint to change the XGameUiTextEntryInputScope value that will be
passed to the window creation function. The value must be a stringified
integer, for example "0" for XGameUiTextEntryInputScope::Default.

This hint is available only if [SDL_GDK_TEXTINPUT](SDL_GDK_TEXTINPUT)
defined.

This hint should be set before calling
[SDL_StartTextInput](SDL_StartTextInput)()

## Version

This hint is available since SDL 3.2.0.

## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

