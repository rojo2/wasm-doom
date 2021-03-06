# WebDOOM

DOOM® is a registered trademark of ZeniMax Media Inc. in the US and/or
other countries. Id Software® is a registered trademark of ZeniMax Media
Inc. in the US and/or other countries. WebDOOM is in no way affiliated
with ZeniMax Media Inc. or id Software LLC and is not approved by ZeniMax
Media Inc. or id Software.

Doom is © 1993-1996 Id Software, Inc.; Boom 2.02 is © 1999 id Software,
Chi Hoang, Lee Killough, Jim Flynn, Rand Phares, Ty Halderman; PrBoom+ is
© 1999 id Software, Chi Hoang, Lee Killough, Jim Flynn, Rand Phares, Ty
Halderman, © 1999-2000 Jess Haas, Nicolas Kalkhof, Colin Phipps, Florian
Schulze, © 2005-2006 Florian Schulze, Colin Phipps, Neil Stevens, Andrey
Budko; Chocolate Doom is © 1993-1996 Id Software, Inc., © 2005 Simon
Howard; Strawberry Doom is © 1993-1996 Id Software, Inc., © 2005 Simon
Howard, © 2008-2010 GhostlyDeath; Crispy Doom is © 2014-2018 Fabian
Greffrath. WebAssembly DOOM is © 2018-2019 Viktor Lázár.

SDL 2.0, SDL_mixer 2.0 and SDL_net 2.0 are © 1997-2016 Sam Lantinga.

Secret Rabbit Code (libsamplerate) is © 2002-2011 Erik de Castro Lopo;
Libpng is © 1998-2014 Glenn Randers-Pehrson, © 1996-1997 Andreas Dilger, ©
1995-1996 Guy Eric Schalnat, Group 42, Inc.; Zlib is © 1995-2013 Jean-loup
Gailly and Mark Adler.

Emscripten is © 2010-2018 Emscripten authors, see [AUTHORS](https://raw.githubusercontent.com/emscripten-core/emscripten/incoming/AUTHORS) file.

# Building

## Development

```sh
emcmake cmake -DCMAKE_BUILD_TYPE=Debug
emmake make -j12
```

## Production

```sh
emcmake cmake -DCMAKE_BUILD_TYPE=Release
emmake make -j12
```

# Controls

Using CTRL and ALT are usually bad choices inside a browser because 
there are a lot of shortcuts that start by using one of those 
modifiers. So, I've changed the controls to be more browser friendly.

- Q: Fire
- E: Use
- WASD: Forward, Strafe Left, Backward, Strafe Right
- Left Arrow: Turn Left
- Right Arrow: Turn Right
- Shift: Run
- Escape: Exit menu
- Enter: Select menu item

# Events

In the original [wasm-doom](https://github.com/lazarv/wasm-doom) there
was a series of undocumented JavaScript events, this is a list of that
events:

- G_DoLoadLevel
- G_DoCompleted
- G_SaveGame
- G_InitNew
- P_KillMobj
- V_ScreenShot
- I_CloseGIF
- I_Error
- I_Endoom

# Missing menu items

I've removed certain menu items because I think they don't make any
sense in a web environment. Those menu items are: Read This! and Quit Game.

Forked & updated with :heart: by [ROJO 2](https://rojo2.com)
