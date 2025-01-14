**In this guide, we'll cover how to build a ESP32s3-based Bluetooth Nugget and combine it with a LoRa backpack to create a Meshtastic node!**

# **Bluetooth Nugget Meshtastic Node**

The **Bluetooth Nugget** is the latest release from the Retia team, updating the previous design with a more powerful esp32s3 microcontroller, flatter screen, better (and more) buttons, neopixel out and i2c ports, and expandable ports for backpacks.

![](https://cdn.shopify.com/s/files/1/2779/8142/files/front.jpg?v=1736486200)![](https://cdn.shopify.com/s/files/1/2779/8142/files/back.jpg?v=1736486200)

The LoRa backpack is a compact, low-power radio add-on ideal for IoT and Meshtastic applications. It supports easy sensor integration and offers software defined power output (+5 to +20 dBm). Designed as a plug-and-play backpack for USB Nugget and Bluetooth Nugget, it works seamlessly with CircuitPython, Arduino, and Meshtastic.

Adding a LoRa backpack to a Bluetooth Nugget allows you to run Meshtastic, and is optimized for adding hardware to support various Meshtastic modules. It allows you to add UART, SPI, and I2C devices, including GPS modules, sensors, RFID readers, and displays.

Designed for applications such as environmental monitoring, presence detection, and remote command execution, it offers reliable communication with minimal power draw.

![](https://cdn.shopify.com/s/files/1/2779/8142/files/backpack.jpg?v=1736486200)

##

## Soldering a Bluetooth Nugget

To put together a Bluetooth Nugget, you'll need the following supplies:

-   1x Bluetooth Nugget PCB with screen
-   1x Wemos S3 Mini board
-   2x low-profile female pin headers
-   Adhesive for mounting the screen (double sided tape)

A Bluetooth Nugget starts without a microcontroller and with the screen flipped to the wrong side. Let's go through the steps of

## Building the Bluetooth Nugget

From the factory, Bluetooth Nuggets come with the screen flipped to the wrong side, and without a microcontroller. Here's how we put one together!

### #1 Adding the screen

First, carefully push both corners of the screen over the ears one by one until the screen is flipped to the front side.

![](https://cdn.shopify.com/s/files/1/2779/8142/files/signal-2025-01-05-233616_480x480.jpg?v=1736149002)

Use a strip of double sided tape to cover the exposed pin headers and adhere the screen into place.

![](https://cdn.shopify.com/s/files/1/2779/8142/files/signal-2025-01-05-233616_002_480x480.jpg?v=1736149002)

Make sure to align the screen properly! It is difficult to move after it's stuck into place.

![](https://cdn.shopify.com/s/files/1/2779/8142/files/signal-2025-01-05-233616_003_480x480.jpg?v=1736149002)

### #2 Adding the Microcontroller

Next, we'll add the esp32s3 based **Wemos S3 Mini** board. We'll also add low-profile female pin headers, which will keep our add-ons fitting correctly. These pin headers are a little hard to find sometimes, but can be bought on Aliexpress.

Here are the dimensions of the pin headers

![](https://cdn.shopify.com/s/files/1/2779/8142/files/H2c0fc6c21c8041ffbe24360d444e8c7f7.webp?v=1736148774)

Here's everything we'll need to finish:

![](https://cdn.shopify.com/s/files/1/2779/8142/files/signal-2025-01-05-233616_004_480x480.jpg?v=1736149002)

First, solder on the low profile pin headers to the top of the microcontroller as seen below. Make sure these are straight, and only solder on a single pin before going any further!

Check the pins are straight, and only solder other pins if you're sure. You can reheat the one soldered pin if you need to straighten them using this technique.

![](https://cdn.shopify.com/s/files/1/2779/8142/files/signal-2025-01-05-233616_006_480x480.jpg?v=1736149002)

In the picture above, a single pin is soldered, allowing me to check to see if the pin headers are on straight. Once they are, solder the rest of the pins.

![](https://cdn.shopify.com/s/files/1/2779/8142/files/signal-2025-01-05-233616_005_480x480.jpg?v=1736149002)

**Final assembly**

**![](https://cdn.shopify.com/s/files/1/2779/8142/files/signal-2025-01-05-233616_007_480x480.jpg?v=1736149002)**

**![](https://cdn.shopify.com/s/files/1/2779/8142/files/signal-2025-01-05-233616_010_480x480.jpg?v=1736149002)**

**![](https://cdn.shopify.com/s/files/1/2779/8142/files/signal-2025-01-05-233616_008_480x480.jpg?v=1736149002)**

Solder the microcontroller on in the direction indicated, making sure not to bridge any of the pins.

Flashing

![](https://cdn.shopify.com/s/files/1/2779/8142/files/signal-2025-01-05-233616_011_480x480.jpg?v=1736149002)

On Nugget.dev, flash the following firmware image:
