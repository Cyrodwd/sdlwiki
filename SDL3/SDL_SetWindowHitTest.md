###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_SetWindowHitTest

Provide a callback that decides if a window region has special properties.

## Header File

Defined in [<SDL3/SDL_video.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h)

## Syntax

```c
bool SDL_SetWindowHitTest(SDL_Window *window, SDL_HitTest callback, void *callback_data);
```

## Function Parameters

|                            |                   |                                                     |
| -------------------------- | ----------------- | --------------------------------------------------- |
| [SDL_Window](SDL_Window) * | **window**        | the window to set hit-testing on.                   |
| [SDL_HitTest](SDL_HitTest) | **callback**      | the function to call when doing a hit-test.         |
| void *                     | **callback_data** | an app-defined void pointer passed to **callback**. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Normally windows are dragged and resized by decorations provided by the
system window manager (a title bar, borders, etc), but for some apps, it
makes sense to drag them from somewhere else inside the window itself; for
example, one might have a borderless window that wants to be draggable from
any part, or simulate its own title bar, etc.

This function lets the app provide a callback that designates pieces of a
given window as special. This callback is run during event processing if we
need to tell the OS to treat a region of the window specially; the use of
this callback is known as "hit testing."

Mouse input may not be delivered to your application if it is within a
special area; the OS will often apply that input to moving the window or
resizing the window and not deliver it to the application.

Specifying NULL for a callback disables hit-testing. Hit-testing is
disabled by default.

Platforms that don't support this functionality will return false
unconditionally, even if you're attempting to disable hit-testing.

Your callback may fire at any time, and its firing does not indicate any
specific behavior (for example, on Windows, this certainly might fire when
the OS is deciding whether to drag your window, but it fires for lots of
other reasons, too, some unrelated to anything you probably care about _and
when the mouse isn't actually at the location it is testing_). Since this
can fire at any time, you should try to keep your callback efficient,
devoid of allocations, etc.

## Version

This function is available since SDL 3.1.3.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

