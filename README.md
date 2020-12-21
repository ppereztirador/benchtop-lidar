# Benchtop Lidar Demo

## Introduction
This code demonstrates the use of the [VL53L1X proximity sensor](https://www.st.com/en/imaging-and-photonics-solutions/vl53l1x.html) in a simple Lidar system.
It includes an Arduino sketch and a Web Serial API-compatible graphic interface for use with the Google Chrome web browser.

## Requisites
The use of this software requires:
- Google Chrome or compatible browser, minimum version 70, ideally version 80 to 88, with the Web Serial API support activated. If the steps in the last section do not work, follow these steps:
    1. Open Google Chrome.
    2. Go to `chrome://flags` from the browser bar.
    3. On the **Search flags** search bar, type `#enable-experimental-web-platform-features`.
    4. Switch the option box near **Experimental Web Platform features** from `Default` to `Enabled`.
    >Be aware that you will need to restart your browser after doing this.
    >
    >By activating experimental features, you might experience compatibility issues with certain web pages. If you are not comfortable leaving it active,
    >switch the flag back to `Disabled` after using the demo.
- The Arduino IDE, downloadable from [Arduino's web site](https://www.arduino.cc/en/software).

## Setup
To setup the Lidar system software, follow these steps:
1. Download **system_code.zip** and extract it in a folder that is easy to find.
2. Program the Arduino:
    1. Open **system_code > system_code.ino**.
    2. Select **Tools > Board > Arduino UNO**
    3. Select **Tools > Port** and choose the port number corresponding to your Arduino. This will typically be the only port available or it will have the name of our board in brackets. Take note of this port name, as it will be used to connect the board to the web interface.
    4. Click the **Upload** button or select **Sketch > Upload** to program the Arduino.
3. Open the web interface:
    - Use the online version in [this link](https://ppereztirador.github.io/lidar_plot) or
    - Use the offline version by following these steps:
        1. Download **lidar_plot.zip** and extract it in a folder that is easy to find.
        2. Go to that folder and open **index.html** in Google Chrome.

## How to use the software
The web interface connects to the Arduino board to start and stop the acquisition of data. Make sure that you have a Google Chrome browser available.

To connect the Arduino board to the web interface:
1. Make sure the USB cable of the Arduino board is connected to the PC.
2. Click the **Connect** button. A box will appear listing the serial ports connected to your computer.
3. Select the Arduino port. This will typically be the same as the one used in the Arduino IDE.
4. The words "Port is now open 🎉" will appear in the bottom of the page if the connection is successful.

To collect and plot data:
1. Click on the **Start** button.
2. The motor should start rotating and the plot will update with the new distances being measured.
3. The new data points will appear in the bottom of the page.
4. To stop the acquisition, click **Stop**.
