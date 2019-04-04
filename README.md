# hackaday_webassembly_demo
Super super simple WebAssembly demo for Hackaday introduction article.
https://hackaday.com/2019/04/04/webassembly-what-is-it-and-why-should-you-care/ 

Compile using Emscripten:
```bash
emcc graphics.c -o graphics.js -O3 -s WASM=1 -s EXTRA_EXPORTED_RUNTIME_METHODS='["cwrap"]'
```

Then run a webserver using something like
```bash
python -m SimpleHTTPServer
```
