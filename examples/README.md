## Device Tree overlay examples for sunxi devices

These are some example overlays for the niche devices (i.e. IIO sensors), custom sensor boards with multiple devices on them or devices that require customization by end user (i.e. SPI displays and touch screens)

Compared to the other ones in this repository these are "standalone" - no fixup script is required, so they can be used with the configfs interface too.

- `sun7i-a20-i2c-edt-ft5x06.dts`: overlay for a touch screen connected to the I2C bus
- `sun8i-h3-gpio-button.dts`: overlay for a GPIO button, active low (when connected to GND), using EINT capable GPIO pin and internal pull-up
- `sun8i-h3-i2c-apds9960.dts`: overlay for an apds9960 sensor connected to the I2C bus
- `sun8i-h3-i2c-pca8574.dts`: overlay fir a PCA8574 GPIO/interrupt controller connected to the I2C bus
- `sun8i-h3-sht1x.dts`: overlay for a Sensirion SHT1x sensor connected to 2 GPIO lines, requires kernel 4.11 or newer
- `sun8i-h3-spi-ad9833.dts`: overlay for a ad9833 DDS function generator with mcp41010 potentiometer (using spidev) located on one board. Requires `spi-add-cs1` overlay on H3 and a kernel patch for ad983x DT bindings (icluded in Armbian)
- `sun8i-h3-double-spidev.dts`: overlay for 2 SPIdev devices on 1 SPI bus. Requires `spi-add-cs1` overlay on H3
