# Benchtop Lidar Demo

## Introduction
This code demonstrates the use of the [VL53L1X proximity sensor](https://www.st.com/en/imaging-and-photonics-solutions/vl53l1x.html) in a simple Lidar system.
It includes an Arduino sketch and a Web Serial API-compatible graphic interface for use with the Google Chrome web browser.

## Requisites
The use of this software requires:
- Google Chrome or compatible browser with the Web Serial API support activated. If the steps in the last section do not work, follow these steps:
  1. Open Google Chrome.
  2. Go to `chrome://flags` from the browser bar.
  3. On the **Search flags** search bar, type `#enable-experimental-web-platform-features`
  4. Switch the option box near **Experimental Web Platform features** from `Default` to `Enabled`.\
  >Be aware that you will need to restart your browser after doing this.
  >
  >By activating experimental features, you might experience compatibility issues with certain web pages. If you are not comfortable leaving it active,
  >switch the flag back to `Disabled` after using the demo.
- The Arduino IDE, downloadable from [here](https://www.arduino.cc/en/software).

## Setup
To setup the Lidar system software, follow these steps:
1. Download **benchtop-lidar.zip** and extract it in a folder that is easy to find.
2. Program the Arduino:
  1. Open **system_code > system_code.ino**. 

## How to use the software


