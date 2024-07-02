testing commit I bugged it
# cool
resources for bunch of stuff I want to learn

# Emacs
- [setting up emacs for IDE experience](https://github.com/rememberYou/.emacs.d/blob/master/config.org#cmake)
- [research workflow](https://emacsconf.org/2021/talks/research/)
- [cool blog on use-package](https://ianyepan.github.io/posts/setting-up-use-package/)
- [crash course on important doom emacs features](https://www.aquabeam.me/tech/doom_emacs_intro/)
- [interesting config](https://babkock.github.io/configs/doom.html)

## Org mode
- [org mode to latex](https://youtu.be/0qHloGTT8XE?si=EL371C1gFZQMDWmD)
- [latex headers](https://jakebox.github.io/youtube/org_latex_video.html)

# Linux stuff
- eww https://elkowar.github.io/eww/eww.html
- waybar https://github.com/Alexays/Waybar/wiki/Module:-Hyprland
- Setup Swaync for notification ?
- [Fabric](https://wiki.ffpy.org/introduction.html)
# AI AND ML
- veryvery cool documentation about a lot of stuff [here](https://willjhliang.github.io/notes/Machine-Learning/PGM/%F0%9F%9A%A8-Bayesian-Network)

# Haskell
- [learning haskell](https://www.cis.upenn.edu/~cis1940/spring13/lectures.html)
# Graphics
## [theoretical stuff](https://www.scratchapixel.com/index.html)
## godot
- [vector math](https://docs.godotengine.org/en/stable/tutorials/math/vector_math.html#doc-vector-math)


## raylib
- [cheatsheet](https://www.raylib.com/cheatsheet/raylib_cheatsheet_v5.0.pdf)
- [raymath](https://www.raylib.com/cheatsheet/raymath_cheatsheet.html)
- [compile to web](https://github-wiki-see.page/m/raysan5/raylib/wiki/Working-for-Web-(HTML5))
   - How I compiled raylib for web:
   - **NOTE** you can write c/c++ then using emscripten to compile to wasm.
   > install emsdk from AUR and setup according to the wiki instructions <br/>
   > cloned raylib into my game directory <br/>
   > in raylib/src <br/>
   > build like this: <br/> ```emcc -c rcore.c -Os -Wall -DPLATFORM_WEB -DGRAPHICS_API_OPENGL_ES2
  emcc -c rshapes.c -Os -Wall -DPLATFORM_WEB -DGRAPHICS_API_OPENGL_ES2
  emcc -c rtextures.c -Os -Wall -DPLATFORM_WEB -DGRAPHICS_API_OPENGL_ES2
  emcc -c rtext.c -Os -Wall -DPLATFORM_WEB -DGRAPHICS_API_OPENGL_ES2
  emcc -c rmodels.c -Os -Wall -DPLATFORM_WEB -DGRAPHICS_API_OPENGL_ES2
  emcc -c utils.c -Os -Wall -DPLATFORM_WEB
  emcc -c raudio.c -Os -Wall -DPLATFORM_WEB```<br/>
   > then `emar rcs libraylib.a rcore.o rshapes.o rtextures.o rtext.o rmodels.o utils.o raudio.o`<br/>
   > you can then go to build directory in raylib and test it by running `cmake ..` <br/>
   > `make`, all examples should work<br/>
   > you MUST build your game file with Async flag ``` emcc -o game.html src/spiral.c -Os -Wall vcpkg/raylib/src/libraylib.a -I./vcpkg/raylib/src -L./vcpkg/raylib/src -s USE_GLFW=3 -s ASYNCIFY --shell-file shell.html -DPLATFORM_WEB```<br/>
   > can then test by running local server `python3 -m http.server 8000`<br/>
   > result: ![image](https://github.com/Haize-uwu/cool/assets/84086558/e9ecd863-d8e2-4b2e-98cd-cdf31003942f)
## Lua Game lib
- [RGlib](https://docs.retrogadgets.game/libs/01-rg_game.html)
## OpenGL
- [wikibook](https://en.wikibooks.org/wiki/OpenGL_Programming/Modern_OpenGL_Introduction)
- [tutorial](https://learnopengl.com/Getting-started/Hello-Triangle)
- [docs](https://www.khronos.org/opengl/wiki/)
## Vulkan
- [Learning Modern 3D Graphics Programming](https://paroj.github.io/gltut/)
- [Vulkan tutorial](https://docs.vulkan.org/tutorial/latest/00_Introduction.html)

# Random
- [stanford thing](https://dawn.cs.stanford.edu/)
- [Online virtual machine](https://bellard.org//jslinux/)
  


---
# Stuff I have actually learnt from this list:
- basic raylib :
  - [window collision and motion](https://imgur.com/a/ztGYED1)
