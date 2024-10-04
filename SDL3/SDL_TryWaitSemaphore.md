###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_TryWaitSemaphore

See if a semaphore has a positive value and decrement it if it does.

## Header File

Defined in [<SDL3/SDL_mutex.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_mutex.h)

## Syntax

```c
bool SDL_TryWaitSemaphore(SDL_Semaphore *sem);
```

## Function Parameters

|                                  |         |                           |
| -------------------------------- | ------- | ------------------------- |
| [SDL_Semaphore](SDL_Semaphore) * | **sem** | the semaphore to wait on. |

## Return Value

(bool) Returns true if the wait succeeds, false if the wait would block.

## Remarks

This function checks to see if the semaphore pointed to by `sem` has a
positive value and atomically decrements the semaphore value if it does. If
the semaphore doesn't have a positive value, the function immediately
returns false.

## Version

This function is available since SDL 3.0.0.

## Code Examples

```c
// BEWARE: This code example was migrated from the SDL2 Wiki, by only updating the names.

void add_data_to_queue(void);
void get_data_from_queue(void);
int data_available(void);
void wait_for_threads(void);

SDL_AtomicInt done;
SDL_Semaphore *sem;
SDL_SetAtomicInt(&done, 0);
sem = SDL_CreateSemaphore(0);

Thread_A:
    while (!SDL_GetAtomicInt(&done)) {
        add_data_to_queue();
        SDL_SignalSemaphore(sem);
    }
Thread_B:
    while (!SDL_GetAtomicInt(&done)) {
        if (SDL_TryWaitSemaphore(sem) == 0 && data_available()) {
            get_data_from_queue();
        }
        /* do other processing */
    }

SDL_SetAtomicInt(&done, 1);
SDL_SignalSemaphore(sem);
wait_for_threads();
SDL_DestroySemaphore(sem);
```

## See Also

- [SDL_SignalSemaphore](SDL_SignalSemaphore)
- [SDL_WaitSemaphore](SDL_WaitSemaphore)
- [SDL_WaitSemaphoreTimeout](SDL_WaitSemaphoreTimeout)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMutex](CategoryMutex)

