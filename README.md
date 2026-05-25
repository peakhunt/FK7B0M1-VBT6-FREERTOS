# The Chinese STM32H7B board with LVGL

Yes the board.

<img src="doc/board.jpg" width="300" alt="The Chinese board">

## Features

## How to Build and Flash

### 1. Clone the Repository
Pull the project and automatically download the pinned LVGL v9.5.0 submodule package:
```bash
git clone --recursive https://github.com/peakhunt/FK7B0M1-VBT6-FREERTOS
cd FK7B0M1-VBT6-FREERTOS
```

### 2. Compile
```bash
make clean
make -j$(nproc)
```

### 3. Flash the Board
Wipes the chip and forces `st-flash` to write past the default 128 KB factory threshold:
```bash
make stflash
```
