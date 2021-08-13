Instructions for installation and using the tag behavior system

# 1. List of devices and materials
|Part|Amount|Price|Link|
|----|------|-----|----|
|RuuviTag| 1 or 2 for each animal | ~33.3-40 Euro |https://ruuvi.com/ruuvitag/|
|Battery for RuuviTag| 1 for 1 tag for 1 year | ~3 Euro |https://ruuvi.com/products/cr2477t-battery/|
|RuuviTag Development Kit| 1 | ~100 Euro |https://ruuvi.com/products/ruuvitag-development-kit/|
||||https://ruuvi.com/products/business-starter-pack/|

# 2. Software installation
## 2.1 Installation of firmware on RuuviTags

## 2.2 Installation of programs on recieving stations Raspberry Pi
### 2.2.2 Setting low energy Bluetooth on Raspberry
sudo apt-get install bluez bluez-hcidump
sudo apt-get install libbluetooth-dev libboost-all-dev cmake git
git clone https://github.com/edrosten/libblepp
cd libblepp
./configure
make -j4
sudo make install

move file libble++.so from /usr/local/lib to /usr/lib

## 2.3 Installation of behavior monitoring program on PC

# 3. Preparation of devices and installation in barn
