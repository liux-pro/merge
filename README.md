# Merge
A component for esp-idf, which merge bootloader,partition table, app and so on to a single one bin file.
# Usage
Run `idf.py merge` , then you can find `esp32.bin` in `build` folder. Burn it to flash at `0x00`.  
The name of bin file may be different based on build target, for example, if you build  firmware for `esp32c3`, you should find `esp32c3.bin`
