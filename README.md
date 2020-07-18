# waveshare_ad_da_board
Firmware for Waveshare AD/DA board

# Prerequisites

1. Download the bcm2835 driver version 1.45. **Note: it is important to use this specific version!** [link](Bcm2835-1.45.tar.gz)
1. Unzip the archive, compile, and install
    ```
    tar xzf Bcm2835-1.45.tar.gz
    cd bcm2835-1.45/
    ./configure
    make
    sudo make check
    sudo make install
    ```
1. Run `sudo raspi-config` and enable SPI, I2C
1. Under root (`sudo su`), run: `echo “device_tree=bcm2710-rpi-3-b.dtb” >> /boot/config.txt`
1. Reboot.


# Compile
```
git clone 
cd cd waveshare_ad_da_board/RaspberryPI/ADS1256/bcm2835/
make clean
make
sudo ./ads1256_test
```
