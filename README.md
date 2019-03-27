# hackaday_webassembly_demo
Super super simple WebAssembly demo for Hackaday introduction article

Compile using Emscripten:
```bash
emcc graphics.c -o graphics.js -O3 -s WASM=1 -s EXTRA_EXPORTED_RUNTIME_METHODS='["cwrap"]'
```

Then run a webserver using something like
```bash
python -m SimpleHTTPServer
```
