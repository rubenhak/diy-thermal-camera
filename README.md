## 

## Hardware

- Raspberry PI 4 B
- [FLIR Radiometric Lepton Dev Kit V2](https://www.sparkfun.com/products/15948)
- [Miuzei Raspberry Pi 4 Touchscreen](https://www.amazon.com/gp/product/B07XBVF1C9)

## Seting up environment

```sh
$ ./build.sh
$ ./run.sh
```

## Running

```sh
$ ./build.sh
$ ./run.sh
```

## Notes

#### DISPLAY ROTATE AND TOUCH SCREEN ICONS.
**NOTE:** causes issues with SPI:

http://www.lcdwiki.com/4inch_HDMI_Display-C

```sh
$ sudo rm -rf LCD-show
$ git clone https://github.com/goodtft/LCD-show.git
$ chmod -R 755 LCD-show
$ cd LCD-show/
$ sudo ./MPI4008-show
```

#### FLIR

```sh
$ sudo apt-get install qt4-dev-tools
$ sudo apt-get -y install git
$ git clone https://github.com/groupgets/LeptonModule.gitcd LeptonModule
$ cd raspberrypi_video
$ qmake && make
```

https://lepton.flir.com/getting-started/lepton-quick-start-raspberry-pi/

https://github.com/groupgets/LeptonModule

https://github.com/groupgets/pylepton


SCREEN & RPI SPI no device issue fix:
https://www.raspberrypi.org/forums/viewtopic.php?t=102171


Not tried:https://groupgets.com/blog/posts/8-installation-guide-for-pure-breakout-board-on-raspberry-pi-2







