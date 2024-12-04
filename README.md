Template for `stm32f407` to use with CMake and CubeMX.
In cube add all that you need. Select to only copy libs that you need (or all of them, whatev).
Select **advanced** app structure, and toolchain `Makefile`.
If you select basic app structure, change `C_SRS` and `INCLUDE_DIRS` in `CMakeLists.txt`.
Double check `CMakeLists.txt` to perhaps remove some unused libs 

Use with something like
```bash
make -j10
make flash
```
