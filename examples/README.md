# Device Tree overlay examples for sunxi devices

These are some example overlays for the niche devices (i.e. IIO sensors), custom sensor boards with multiple devices on them or devices that require customization by end user (i.e. SPI displays and touch screens)

- `sun7i-a20-i2c-edt-ft5x06.dts`: overlay for a touch screen connected to I2C bus
- `sun8i-h3-i2c-apds9960.dts`: overlay for an apds9960 sensor connected to I2C bus
- `sun8i-h3-spi-ad9833.dts`: overlay for a ad9833 DDS function generator with mcp41010 potentiometer (using spidev) located on one board. This is an example of connecting a 2 SPI devices to 1 SPI bus on H3 based boards
- `sun8i-h3-sht1x.dts`: overlay for a Sensirion SHT1x sensor connected to 2 GPIO lines
