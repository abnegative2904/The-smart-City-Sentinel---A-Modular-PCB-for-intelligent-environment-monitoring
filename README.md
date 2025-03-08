# The Smart City Sentinel - A Modular PCB for Intelligent Environment Monitoring

![PCB Design](https://github.com/abnegative2904/The-smart-City-Sentinel---A-Modular-PCB-for-intelligent-environment-monitoring/blob/main/pcb-design.jpg?raw=true)

##Footprints are missing for some components
![SCHEMATIC](https://github.com/user-attachments/assets/c090c716-13ba-4904-8b2f-326504511ece)

## 1. Power Supply:
   - The system is powered by a solar panel and a rechargeable battery, managed by a TP4056 module.
   - A voltage booster ensures components needing 5V are powered correctly.
   - The ESP32-C3 monitors the battery level. When the battery is low, it charges through the solar panel.

## 2. Data Collection:
   - *Air Quality:* The MQ-135 sensor detects harmful gases.
   - *Temperature, Humidity, and Pressure:* The BME280 and DHT11 sensors gather environmental data.
   - *Sound Levels:* A sound sensor measures ambient noise.
   - *Dust and Particulate Matter:* A dust sensor monitors air quality.
   - *Additional Sensors:* Hall effect, water flow, soil moisture, and rain sensors provide more data.

## 3. Data Processing:
   - The ESP32-C3 processes data from all sensors. It uses the DS3231 RTC module to timestamp the data for accurate logging.

## 4. Display and Output:
   - An OLED display shows real-time data for easy monitoring.
   - A relay module can control external devices based on sensor readings (e.g., turning on a fan if air quality is poor).

## 5. Communication:
   - I2C communication is used for the OLED display, RTC, and BME280 sensor.
   - The system can send data to a server or cloud for remote monitoring and analysis.

This setup provides a comprehensive solution for monitoring environmental conditions, making it ideal for applications like smart agriculture, home automation, and environmental research.
