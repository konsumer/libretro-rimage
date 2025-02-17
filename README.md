# libretro-rimage

A proof-of-concept of using libretro with raylib's Image API [rimage](https://github.com/robloach/rimage).

## Example

```
ClearBackground(SKYBLUE);
ImageDrawCircle(&core->backBuffer, 200, 150, 30, RED);
ImageDrawRectangle(&core->backBuffer, 400, 200, 100, 140, GREEN);
ImageDrawLine(&core->backBuffer, 50, 300, 550, 380, ORANGE);
```

## Development

```
cmake -B build .
make -C build

# linux
retroarch -L build/rimage_libretro.so

# mac
/Applications/RetroArch.app/Contents/MacOS/RetroArch -L build/rimage_libretro.dylib

# windows
retroarch -L build/rimage_libretro.dll
```

## License

[zlib](LICENSE)
