# Homeassitant Waveshare e-Paper 7.5 inch

<br>

![e-Paper Display](/assets/DSC05657.png)

<br>

---

## Preface:

Time to say **Thank You** to the Homeassitant community for inspiration and support this year. I was able to learn a lot thanks to great people and would like to give something back to you here.

The motivation for this project is due to the defect of my weather station and thus the end of the weather display in the living room. Since we were lacking this information, I decided to bundle the Smart Home components and also information from my data science work.<br>
So it was obvious to set up the new information centre in the living room using ESPHome and Homeassistant.

Have fun with tinkering and programming... **:)**
<br><br>

#### Disclaimer:

"Rebuilding is done at your own risk. I assume no liability for any damage caused by the replica.
Hardware replication is done at your own responsibility and risk and it is recommended that all necessary steps are taken to protect property and self safety.
I assume no liability for consequential damages resulting from reverse engineering."
<br><br>

## Information Features

- [Dates of the waste collection HA-Intergration](https://youtu.be/aCKLKGYiA7w)
- Heating oil prices German Market (Data via Webscraping)
- Current oil tank content (Coming soon: [Lidar-Sensor in progress]())
- Petrol prices of the nearest petrol stations
- Sunrise / Sunset
- CO2
- Weather Forecast from HA Integration
- Rain last 24H (Symbol shows if it is raining or not)
- Actual Windspeed ( min/max)
- Wind Direction Text (NO,NE...) and Value in °
- Moon Phase (from HA Integration)
- uptime
- Wlan Indicator
- Living Room Temperature
- Outside Temperature (min + max)
- Windchill Temperature
- Time, Weekday, Calendar Week

<br><br>

## Hardware:

- Raspi4 & Homeassistant

- [Product e-Paper esp32 ](https://www.waveshare.com/e-paper-esp32-driver-board.htm)

- [Wiki-e-Paper_ESP32_Driver_Board](http://www.waveshare.com/wiki/E-Paper_ESP32_Driver_Board)

- [7.5inch E-Paper (B) E-Ink Raw Display, 800×480](https://www.waveshare.com/7.5inch-e-paper-b.htm) (Color not used at this Revision)
- Picture Frame
- 3D printed Case for ESP32 Driver Board ![3D printed Case](/3D/Case.jpeg)
- [Box STL](./3D/Case_esp32.stl)

<br><br>

## Software

- Homeassistant (HA)
- ESPHome

<br><br>

## Preparation:

- Download [OpenSansBold.ttf](https://fonts.google.com/specimen/Open+Sans) and [materialdesignicons-webfont.ttf](https://github.com/Templarian/MaterialDesign-Webfont/raw/master/fonts/materialdesignicons-webfont.ttf)
- Copy \*.ttf files to /config/esphome/fonts/ Folder on your HA Instance
- Create new ESPHome Device copy [yaml Code](/yaml/waveshare-disp.yaml)
- Adapt/Check Names of your HA Sensors
- **Register in HA under Settings/Devices&Services/** -> ADD New Intergration; Search ESPHome and follow the Instructions.
- Test your installation and adjust parameters as you like.. ::smile::
  <br><br>

## Note:

- This e-Paper Display supports no partial refresh
- Currently, possible colors of the display are not used
- Display information refreshed every 5 minutes
