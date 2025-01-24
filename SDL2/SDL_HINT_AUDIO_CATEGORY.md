# SDL_HINT_AUDIO_CATEGORY

A variable controlling the audio category on iOS and Mac OS X

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_AUDIO_CATEGORY   "SDL_AUDIO_CATEGORY"
```

## Remarks

This variable can be set to the following values:

- "ambient": Use the AVAudioSessionCategoryAmbient audio category, will be
  muted by the phone mute switch (default)
- "playback": Use the AVAudioSessionCategoryPlayback category

For more information, see Apple's documentation:
https://developer.apple.com/library/content/documentation/Audio/Conceptual/AudioSessionProgrammingGuide/AudioSessionCategoriesandModes/AudioSessionCategoriesandModes.html





----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

