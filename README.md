# merge
A component for esp-idf ,which merge bootloader,nvs,partition table etc. bin file into single one.
# use
Run `idf.py merge` , then you can find `esp32.bin` in `build` folder. Burn it to flash at `0x00`.  
The name of bin file may be different based on build target, for example, if you build  firmware for `esp32c3`, you should find `esp32c3.bin`