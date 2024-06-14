# Installing raylib and getting it to work on Wayland

- cloned the repo over at
  ```
  git clone https://github.com/raysan5/raylib.git raylib
  cd raylib
  ```
- build using cmake ` cmake -DBUILD_SHARED_LIBS=ON -DUSE_WAYLAND=ON ..`
  - NOTE: I am using openGL version 4.6 but left raylib to build with defaults
- then `make`
- finally ` sudo make install `

  In Build/examples all exmaples work correctly including the shader and lighting examples that were buggy

  Will Include a make file for general builds...
