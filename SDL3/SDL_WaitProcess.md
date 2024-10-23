###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_WaitProcess

Wait for a process to finish.

## Header File

Defined in [<SDL3/SDL_process.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_process.h)

## Syntax

```c
bool SDL_WaitProcess(SDL_Process *process, bool block, int *exitcode);
```

## Function Parameters

|                              |              |                                                                                        |
| ---------------------------- | ------------ | -------------------------------------------------------------------------------------- |
| [SDL_Process](SDL_Process) * | **process**  | The process to wait for.                                                               |
| bool                         | **block**    | If true, block until the process finishes; otherwise, report on the process' status.   |
| int *                        | **exitcode** | a pointer filled in with the process exit code if the process has exited, may be NULL. |

## Return Value

(bool) Returns true if the process exited, false otherwise.

## Remarks

This can be called multiple times to get the status of a process.

The exit code will be the exit code of the process if it terminates
normally, a negative signal if it terminated due to a signal, or -255
otherwise. It will not be changed if the process is still running.

## Thread Safety

This function is not thread safe.

## Version

This function is available since SDL 3.1.3.

## See Also

- [SDL_CreateProcess](SDL_CreateProcess)
- [SDL_CreateProcessWithProperties](SDL_CreateProcessWithProperties)
- [SDL_KillProcess](SDL_KillProcess)
- [SDL_DestroyProcess](SDL_DestroyProcess)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryProcess](CategoryProcess)

