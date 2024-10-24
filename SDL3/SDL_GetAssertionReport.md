###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetAssertionReport

Get a list of all assertion failures.

## Header File

Defined in [<SDL3/SDL_assert.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_assert.h)

## Syntax

```c
const SDL_AssertData * SDL_GetAssertionReport(void);
```

## Return Value

(const [SDL_AssertData](SDL_AssertData) *) Returns a list of all failed
assertions or NULL if the list is empty. This memory should not be modified
or freed by the application. This pointer remains valid until the next call
to [SDL_Quit](SDL_Quit)() or
[SDL_ResetAssertionReport](SDL_ResetAssertionReport)().

## Remarks

This function gets all assertions triggered since the last call to
[SDL_ResetAssertionReport](SDL_ResetAssertionReport)(), or the start of the
program.

The proper way to examine this data looks something like this:

```c
const SDL_AssertData *item = SDL_GetAssertionReport();
while (item) {
   printf("'%s', %s (%s:%d), triggered %u times, always ignore: %s.\\n",
          item->condition, item->function, item->filename,
          item->linenum, item->trigger_count,
          item->always_ignore ? "yes" : "no");
   item = item->next;
}
```

## Thread Safety

This function is not thread safe. Other threads calling
[SDL_ResetAssertionReport](SDL_ResetAssertionReport)() simultaneously, may
render the returned pointer invalid.

## Version

This function is available since SDL 3.1.3.

## Code Examples

The proper way to examine this data looks something like this:
```c
const SDL_AssertData *item = SDL_GetAssertionReport();
while (item) {
     printf("'%s', %s (%s:%d), triggered %u times, always ignore: %s.\n",
          item->condition, item->function, item->filename,
          item->linenum, item->trigger_count,
          item->always_ignore ? "yes" : "no");
     item = item->next;
}
```

## See Also

- [SDL_ResetAssertionReport](SDL_ResetAssertionReport)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAssert](CategoryAssert)

