# Changelog

## 1.0.0
- ESPHome firmware for the Smogomierz hardware (NodeMCU + PMS7003, same wiring).
- SHT45 for temperature and humidity, BME280 for pressure, optional BH1750.
- PMS7003 sleeps between readings (120 s), sea-level pressure, dew point,
  "PM readings unreliable" in fog.
- Optional Sensor.Community upload (PMS7003 pin 1, BME280 pin 11).
