# SDL_GetThreadID

Get the thread identifier for the specified thread.

## Header File

Defined in [<SDL3/SDL_thread.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_thread.h)

## Syntax

```c
SDL_ThreadID SDL_GetThreadID(SDL_Thread *thread);
```

## Function Parameters

|                            |            |                      |
| -------------------------- | ---------- | -------------------- |
| [SDL_Thread](SDL_Thread) * | **thread** | the thread to query. |

## Return Value

([SDL_ThreadID](SDL_ThreadID)) Returns the ID of the specified thread, or
the ID of the current thread if `thread` is NULL.

## Remarks

This thread identifier is as reported by the underlying operating system.
If SDL is running on a platform that does not support threads the return
value will always be zero.

## Version

This function is available since SDL 3.2.0.

## Code Examples

```c
#include <SDL3/SDL.h>
#include <SDL3/SDL_main.h>

// Very simple thread - counts 0 to 9 delaying 50ms between increments
int TestThread(void *ptr)
{
    int cnt;

    for (cnt = 0; cnt < 10; ++cnt) {
        SDL_Log("Thread counter: %d", cnt);
        SDL_Delay(50);
    }

    return cnt;
}

int main(int argc, char *argv[])
{
    SDL_Thread   *thread;
    SDL_ThreadID threadID;
    int          threadReturnValue;

    SDL_Log("Simple SDL_CreateThread test:");

    /* Simply create a thread */
    thread = SDL_CreateThread(TestThread, "TestThread", (void *)NULL);

    if (!thread) {
        SDL_LogError(SDL_LOG_CATEGORY_APPLICATION, "SDL_CreateThread failed: %s\n", SDL_GetError());
        return -1;
    }

    /* Retrieve the ID for the newly launched thread */
    threadID = SDL_GetThreadID(thread);

    /* Wait for the thread to complete and get the return code */
    SDL_WaitThread(thread, &threadReturnValue);
    SDL_Log("Thread returned value: %d", threadReturnValue);

    return 0;
}
```

## See Also

- [SDL_GetCurrentThreadID](SDL_GetCurrentThreadID)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryThread](CategoryThread)

