# TrisWebAssembly
This is my first project where I took advantage of the WebAssembly.
The game in question is the tic-tac-toe, the logic was made in C ++. I took advantage of a part of the project made during university and readjusted it with emscripten.

## Requirements
To start the project you need:
- install emscripten
- build the project
- set up a local server in python3 to avoid CORS problems

### Install emscripten
follow the guide here
https://emscripten.org/docs/getting_started/downloads.html

### Build the project 
now you need to build to get the tris.wasm file by running this command
```emcc --bind -o tris.js tris.cpp```

### Set up a local server in python3
execute the command ```python3 -m http.server```
go to the browser and type /tris after localhost:port
