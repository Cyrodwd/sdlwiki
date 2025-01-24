# SDL_HINT_PREFERRED_LOCALES

Override for [SDL_GetPreferredLocales](SDL_GetPreferredLocales)()

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_PREFERRED_LOCALES "SDL_PREFERRED_LOCALES"
```

## Remarks

If set, this will be favored over anything the OS might report for the
user's preferred locales. Changing this hint at runtime will not generate a
[SDL_LOCALECHANGED](SDL_LOCALECHANGED) event (but if you can change the
hint, you can push your own event, if you want).

The format of this hint is a comma-separated list of language and locale,
combined with an underscore, as is a common format: "en_GB". Locale is
optional: "en". So you might have a list like this: "en_GB,jp,es_PT"





----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

