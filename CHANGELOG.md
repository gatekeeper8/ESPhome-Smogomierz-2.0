# Changelog

## 1.1.0
- Readings are rounded on the device before they are sent (`round` filter), so Home
  Assistant, its history and Sensor.Community get e.g. `2.25 °C` instead of the raw
  float `2.2517874…`: temperature 2 decimals, humidity, pressure, sea-level pressure
  and dew point 1 decimal. `accuracy_decimals` alone only changed the display.
- PM measured every 5 minutes instead of 2 (`pm_interval: 300s`): the PMS7003 fan and
  laser run far less, so the sensor lasts longer and heats the box less.
- README: keep the SHT45 outside the box; the measured warming inside it.

## 1.0.0
- ESPHome firmware for the Smogomierz hardware (NodeMCU + PMS7003, same wiring).
- SHT45 for temperature and humidity, BME280 for pressure, optional BH1750.
- PMS7003 sleeps between readings (120 s), sea-level pressure, dew point,
  "PM readings unreliable" in fog.
- Optional Sensor.Community upload (PMS7003 pin 1, BME280 pin 11).
