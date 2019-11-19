#### WebAssembly Integrate Library by EMCC


Easy Starter by developers.google.com [🔗](https://developers.google.com/web/updates/2018/03/emscripting-a-c-library)

- Usage:
  - ```chmod 755 compile.sh```
  - ```./compile.sh```
  - ```python -m http.server 8001```
- Library: Libwebp
- Key: 
  - ```emcc -I libwebp libwebp/src/{dec,dsp,demux,enc,mux,utils}/*.c``` 

> Note: This strategy will not work with every C project out there. Many projects rely on autoconf/automake to generate system-specific code before compilation. Emscripten provides emconfigure and emmake to wrap these commands and inject the appropriate parameters. You can find more in the Emscripten documentation/Emmake and Emconfigure