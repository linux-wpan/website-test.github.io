Supported Hardware
------------------

Table 1. Supported 802.15.4 Hardware

Transceiver | Supported | Driver | Bus | Where to buy
----------- | --------- | ------ | --- | ------------
adf7242 | yes | adf7242 | SPI or PMOD | [Analog](http://www.analog.com/en/products/rf-microwave/integrated-transceivers-transmitters-receivers/low-power-rf-transceivers/adf7242.html#product-samplebuy)
at86rf212 | yes | at86rf230 | SPI | [aliexpress](http://de.aliexpress.com/item/Wireless-transceiver-module-zigbee-module-belt-at86rf212-mcu-chip-780m-module/1757611944.html)
at86rf212b | yes | at86rf230 | SPI | [digikey](http://www.digikey.com/product-search/en?x=0&y=0&lang=en&site=us&keywords=ATZB-212B-XPRO)
at86rf230 | no | at86rf230? | SPI
at86rf231 | yes | at86rf230 | SPI | [atben](http://downloads.qi-hardware.com/people/werner/wpan/web/) Out of stock. Mailto linux-wpan and Werner to produce maybe new ones. Or contact [qi-hardware](http://en.qi-hardware.com/wiki/Main_Page).
at86rf233 | yes | at86rf230 | SPI | [openlabs](http://openlabs.co/store/Raspberry-Pi-802.15.4-radio), [digikey](http://www.digikey.com/product-search/en?x=0&y=0&lang=en&site=us&keywords=ATREB233-XPRO)
atusb | yes | atusb | USB | [Sysmocom](http://shop.sysmocom.de/products/atusb)
ca8210 | yes | ca8210 |  SPI | [Cascoda](https://www.cascoda.com/buy/)
cc2420 | no | |  SPI | [aliexpress](http://de.aliexpress.com/store/product/ZIGBEE-networking-technology-Wi-Fi-CC2420-wireless-transceiver-modules-including-antenna/1383438_2036388706.html)
cc2520 | yes | cc2520 | SPI | [aliexpress](http://de.aliexpress.com/item/CC2520-wireless-module-ZIGBEE-wireless-sensor-networking-module-with-SMA-external-antenna/1921436550.html)
cc2531 | no | | USB | [aliexpress](http://de.aliexpress.com/item/free-shipping-FOR-ZigBee-CC2531-USB-dongle-protocol-analysis-port-capture-wireless-keyboard-and-mouse/32270975591.html)
mcr20a | yes | mcr20a | SPI | [NXP](https://www.nxp.com/products/wireless-connectivity/thread/2.4-ghz-802.15.4-wireless-transceiver:MCR20A)
mrf24j40 | yes | mrf24j40 | SPI | [aliexpress](http://de.aliexpress.com/item/MRF24J40MA-I-RM-MRF24J40MA-I-MRF24J40MA-MRF24J40-MICROC-QFN-Import-original/32223258627.html)
RZUSBstick | experimental, [WIP](http://wpan.cakelab.org/firmwares/rzusb.bin) | atusb | USB | [element14](http://www.element14.com/community/docs/DOC-67532/l/avr-rz-usb-stick-module)
Xbee | no | [out of tree](https://github.com/joaopedrotaveira/linux-rpl/blob/master/mainline-3.12.y/0001-Added-XBee-driver-support.patch) | ?? | [sparkfun](https://www.sparkfun.com/pages/xbee_guide)

Table 2. Boards with Transceivers

Name | Transceiver | Website
---- | ----------- | -------
Ci40 | ca8210 | [kickstarter](https://www.kickstarter.com/projects/imgtec/creator-ci40-the-ultimate-iot-in-a-box-dev-kit)
blixten | cc2520 | [jopee](https://jopee.wordpress.com/6lowpan-gateway/)
