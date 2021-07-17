This repo shows you how to run a Hello World app for a nRF52 device using Renode

**Prerequisites:**
* Install Renode
    * [1.12 Release](https://github.com/renode/renode/releases/tag/v1.12.0)
    * Make sure to include on PATH
* Clone this repo
* [Install cross compiler](https://armkeil.blob.core.windows.net/developer/Files/downloads/gnu-rm/9-2019q4/gcc-arm-none-eabi-9-2019-q4-major-win32-sha2.exe)
* Install GNU  Make (I used MSYS2)

**Notes**
Only tested on Windows 10 

**Build and Run**
Run make to recreate the included elf file
`cd ./src/hello_world/pca10056/blank/armgcc/makefile`
`make`

**Run Renode Default Zephyr Project** 
`renode --console -e "i @scripts/nrf52840.resc; s"`

**Run Hello World Build**
`renode --console -e "i @scripts/hello_world.resc; s"`

Look for the "Hello, World!" output in the UART0 window.