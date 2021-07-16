This repo shows you how to create a Hello World project for an nRF52 device and simulate it using Renode.

**Prerequisites:**
* Install Renode
    * [1.12 Release](https://github.com/renode/renode/releases/tag/v1.12.0)
    * Make sure to include on PATH
* Clone this repo
* Run the appropriate script for your OS from the /scripts dir
* nRF SDK https://www.nordicsemi.com/Products/Development-software/nRF5-SDK/Download#infotabs

**Run Rednode Default Zephyr Project** 
`renode --console -e "i @scripts/nrf52840.resc; s"`

**Run Hello World Script**
`renode --console -e "i @scripts/hello_world.resc; s"`