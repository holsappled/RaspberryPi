# RaspberryPi
## Arducam releases new Arducam Mini cameras drivers for Raspberry Pi platform.
- Optimized the speed of SPI and Improved image transmission speed
- Support for Arducam Mini 2MP/2MP Plus/5MP/5MP Plus
- Support for 4 cameras work together
- Support for transering image data through the wifi.
## Pins definition (BCM)
```Bash
//ArduCAM CS pins
#define     CAM_CS1         17
#define     CAM_CS2         23
#define     CAM_CS3         22
#define     CAM_CS4         24
```
```Bash
//I2c pins
#define sda_port        2 
#define scl_port        3
```
```Bash 
//SPI pins 
//set 9 (MISO), 10 (MOSI), 11 (SCLK) alt fxn 0 (SPI0)
```

## Platform configuration (bcm283x_board_driver.h)
- These #define values are specific to the BCM2835, taken from "BCM2835 ARM Peripherals"
```Bash
#define BCM2835_PERI_BASE        0x20000000
```
- Updated to BCM2836 for Raspberry Pi 2.0 
```Bash
#define BCM2835_PERI_BASE        0x3F000000
```

## Quickly start
```bash
sudo git clone https://github.com/ArduCAM/RaspberryPi.git
```
```bash 
cd RaspberryPi/
```
```bash
sudo make 
```
```bash
sudo ./run_Arducam_Demo 
```
![Alt text](https://github.com/ArduCAM/RaspberryPi/blob/master/data/image1.png)



