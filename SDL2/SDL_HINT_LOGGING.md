# SDL_HINT_LOGGING

A variable controlling the default SDL log levels.

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_LOGGING   "SDL_LOGGING"
```

## Remarks

This variable is a comma separated set of category=level tokens that define
the default logging levels for SDL applications.

The category can be a numeric category, one of "app", "error", "assert",
"system", "audio", "video", "render", "input", "test", or `*` for any
unspecified category.

The level can be a numeric level, one of "verbose", "debug", "info",
"warn", "error", "critical", or "quiet" to disable that category.

You can omit the category if you want to set the logging level for all
categories.

If this hint isn't set, the default log levels are equivalent to:
"app=info,assert=warn,test=verbose,*=error"

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

