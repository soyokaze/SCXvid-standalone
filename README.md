## SCXvid-standalone
Standalone, cross-platform port of [the AviSynth SCXvid plugin][1].

### Usage
```
scxvid output.log < input.y4m
```
Only 4:2:0 input is supported.
### Downloads
Win32 executable can be found in the releases section. For *nix you'll have to build it from source.
### Building
#### Requirements
* Xvid 1.3.x

#### On Windows
Use the Visual Studio solution in the repository. The "xvidcore" directory from Xvid sources must be on the same level with SCXvid directory. Also make sure that you compile libxvidcore with DLL runtime, not static.
#### On Unix-like systems
Assuming you have libxvidcore properly installed somewhere in compiler's default paths, run:
```
cc -lxvidcore -o scxvid scxvid.c
```


[1]: https://code.google.com/p/yatta-ivtc/source/browse/#svn%2Fscxvid%2Ftrunk
