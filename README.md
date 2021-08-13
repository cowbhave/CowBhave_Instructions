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
Connect the RuuviTag Development Kit to a PC according to the instructions:

https://lab.ruuvi.com/devshield/
https://ruuvi.com/setting-up-the-development-environment-for-ruuvitag-firmware/


## 2.2 Installation of programs on recieving stations Raspberry Pi
Install Raspberry Pi OS according to the instructions:
https://www.raspberrypi.org/software/


### 2.2.2 Setting low energy Bluetooth on Raspberry Pi

> sudo apt-get install bluez bluez-hcidump

> sudo apt-get install libbluetooth-dev libboost-all-dev cmake git
> git clone https://github.com/edrosten/libblepp

cd libblepp

./configure

make -j4

sudo make install


move file libble++.so from /usr/local/lib to /usr/lib

### 2.2.3 Setting ZeroMQ for C++ on Raspberry Pi
Installing according to the instructions at https://github.com/MonsieurV/ZeroMQ-RPi

cd ..

sudo apt-get install libtool pkg-config build-essential autoconf automake

sudo wget https://github.com/jedisct1/libsodium/releases/download/1.0.3/libsodium-1.0.3.tar.gz

sudo tar -zxvf libsodium-1.0.3.tar.gz

cd libsodium-1.0.3/

sudo ./configure

sudo make

sudo make install

cd ..

sudo wget http://download.zeromq.org/zeromq-4.1.3.tar.gz

sudo tar -zxvf zeromq-4.1.3.tar.gz

cd zeromq-4.1.3/

./configure

make

sudo make install

sudo ldconfig

cd /usr/include/

sudo wget https://raw.githubusercontent.com/zeromq/cppzmq/master/zmq.hpp



## 2.3 Installation of behavior monitoring program on PC

# 3. Preparation of devices and installation in barn

# 4. Examples for cost estimation

### 4.1 Barn with 100 cows

### 4.2 Barn with 20 cows
