# lora-pi-hat
Raspberry Pi HAT for mPCIe LoRa gateway cards

Untested
* jumpers are probably unnecessary because SPI pins are independent
* u-blox module can be swapped for *much* cheaper alternative
* gateway current consumption @3.3V ~ 500mA, DC/DC designed for 1A

| Pin | mini PCIe  | MTAC        | RAK      |
|-----|------------|-------------|----------|
| 1   | WAKE#      |             |          |
| 2   | 3.3Vaux    | VDD_3V3     | VDD_3V3  |
| 3   | COEX1      |             |          |
| 4   | GND        | GND         | GND      |
| 5   | COEX2      | SPI_MOSI    |          |
| 6   | 1.5Vaux    |             |          |
| 7   | CLKREQ#    | SPI_MISO    |          |
| 8   | UIM_PWR    |             |          |
| 9   | GND        | GND         | GND      |
| 10  | UIM_DATA   |             |          |
| 11  | REFCLK-    |             |          |
| 12  | UIM_CLK    | SPI_NCS     |          |
| 13  | REFCLK+    | SPI_CLK     |          |
| 14  | UIM_RESET  | ?           |          |
| 15  | GND        | GND         | GND      |
| 16  | UIM_VPP    |             |          |
| 17  | Reserved   |             |          |
| 18  | GND        | GND         | GND      |
| 19  | Reserved   |             | GPS_PPS  |
| 20  | W_DISABLE# |             |          |
| 21  | GND        | GND         | GND      |
| 22  | PERST#     | RESET       | RESET    |
| 23  | PERn0      | VDD_5V      |          |
| 24  | 3.3Vaux    | VDD_3V3     | VDD_3V3  |
| 25  | PERp0      | VDD_5V      |          |
| 26  | GND        | GND         | GND      |
| 27  | GND        | EEPROM_A1   | GND      |
| 28  | 1.5Vaux    | GPS_PPS     |          |
| 29  | GND        | EEPROM_A2   | GND      |
| 30  | SMB_CLK    | I2C_SCL     |          |
| 31  | PETn0      |             |          |
| 32  | SMB_DATA   | I2C_SDA     |          |
| 33  | PETp0      |             |          |
| 34  | GND        | GND         | GND      |
| 35  | GND        | GND         | GND      |
| 36  | USB_D-     |             |          |
| 37  | GND        | GND         | GND      |
| 38  | USB_D+     |             |          |
| 39  | 3.3Vaux    | VDD_3V3     | VDD_3V3  |
| 40  | GND        | GND         | GND      |
| 41  | 3.3Vaux    | VDD_3V3     | VDD_3V3  |
| 42  | LED_WWAN#  | ?           |          |
| 43  | GND        | GND         | GND      |
| 44  | LED_WLAN#  |             |          |
| 45  | Reserved   |             | SPI_CLK  |
| 46  | LED_WPAN#  |             |          |
| 47  | Reserved   |             | SPI_MISO |
| 48  | 1.5Vaux    |             |          |
| 49  | Reserved   |             | SPI_MOSI |
| 50  | GND        | GND         | GND      |
| 51  | Reserved   |             | SPI_NCS  |
| 52  | 3.3Vaux    | VDD_3V3     | VDD_3V3  |
