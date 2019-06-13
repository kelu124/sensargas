# Sensargas


	
	
	

# Review of objectives

* Mesure presence of Sargasse algae
  * Main measure : H2S
    * Requires : secondary measures : temp / humidity (for calibration)
  * What about cheap secondary measurements if cheap ?
* Participatory ?
  * Arduino-IDE use
  * Sensors on the market
* Communicates outside
  * Wifi -> onboard, requires internet access pont
  * Bluetooth -> onboard, low range
  * LoRa -> Sparse network, but more pins required, more power, more elements
* Cheap
* Identification 
  * to be able to locate a captor on a map
* Low-energy
  * Energy harvesting ? Solar or .. ? -> low solar power possibly, introduces not reliaiblity
  * Use battery
    * Li-Ion
    * CR2024 rechargeable cell
    * 18655 cell ?
    * What about supercap ?
  * Battery measurement needed ?
  
# Methodo

## 1. Define architecture

* Do devkit
* Test

## 2. PréPCB

* Orders

# Exploring

## Sensors


### Dust

* Dust sensor - Sharp Optical Dust Sensor
  * https://github.com/Trefex/arduino-airquality
* DSM501 a DSM501A dust sensor 
  * https://github.com/alexjx/AqiMon

### Humidity / temperature

* SHT10 by sensiron/DFRobot
  * https://github.com/Trefex/arduino-airquality

### Carbon monoxide

* Carbon monoxide sensor - Parallax CO sensor
  * https://github.com/Trefex/arduino-airquality

### Barometric

* BMP085 Barometric Pressure/Temperature/Altitude Sensor
  * https://github.com/Trefex/arduino-airquality
* BME280 simple but high resolution pressure/humidity/temperature sensor

### PM

* PMS5003 - PM1.0, PM2.5 and PM10.0 - 40$
  * https://www.adafruit.com/product/3686
  * Sensor: PM2.5 (0.3 – 10um)
### VOCs - 

* CCS811 - TVOCs (20$)
  * Volatile Organic Compounds (TVOCs), including equivalent carbon dioxide (eCO2) and metal oxide (MOX) levels
  * https://www.sparkfun.com/products/14193
  * i2c
  * https://github.com/codmpm/esp-ccs811-bme280-mqtt for MQTT lib
  * https://github.com/kriswiner/CCS811
* SGP30 - 20$
  * Sensor: eCO2 (0-60,000 ppm)
  * Sensor: TVOC (0-60,000 ppb


### Air Quality General

* MQ135 - 2$
  * CO2, à l’alcool, au Benzène, à l’oxyde d’azote (NOx) et à l’ammoniac (NH3)
  * Needs temperature / humidity measurement
  * Calibration : https://github.com/zesteros/ArduinoAirQualityMonitor

## Similar low energy / specs projects

* https://hackaday.io/project/27560-low-costpowersize-temperature-logger
* https://www.tindie.com/products/kdcircuits/trigboard-ultra-low-power-esp8266-iot-platform/

## Power use:

* https://openhomeautomation.net/power-monitoring-arduino-ina219
* Charging cap with solar : 
  * https://www.gammon.com.au/forum/?id=12821
* https://hallard.me/bp-ulpnode/
  * CR2450 or CR2032 Cell Coin
* https://hackaday.com/2013/08/04/measuring-tiny-current-with-high-resolution/

* http://www.home-automation-community.com/arduino-low-power-how-to-run-atmega328p-for-a-year-on-coin-cell-battery/
* Interesting : https://www.element14.com/community/thread/49699/l/new-ultra-low-power-arduino-board-with-built-in-rf-rfm69?displayFullThread=true
* Tres interessant: https://hackaday.com/2018/11/13/low-energy-esp8266-based-board-sleeps-like-a-log-until-triggered/

# Funding sources

* Mairies de Paris
* Voirie (capteurs H2S existants)
* Saint Brieuc pour algues vertes
* Caraibes -> communes

# How: participatory approach

## Us ?

## Other projects

* http://fablab.sorbonne-universites.fr/wiki/doku.php?id=wiki:projets:open-air 
* http://fablab.sorbonne-universites.fr/wiki/doku.php?id=wiki:projets:open-air:proto
* https://bral.brussels/fr/artikel/projet-expair-citizens-demand-clean-air
* http://www.mobicitair.fr/
* http://aircitizen.org/
* http://www.wiki-rennes.fr/Ambassad%27Air 


* http://imu.universite-lyon.fr/projet/urpolsens-reseaux-de-capteurs-sans-fil-pour-le-suivi-de-la-pollution-urbaine-wireless-sensor-networks-for-urban-pollution-monitoring/ 
* https://pad.lamyne.org/s/BkVyZ4RNf
* https://atmo-france.org/mesure-de-la-qualite-de-lair-une-action-citoyenne/
* https://www.ville-antony.fr/bp2018-capteurs-qualite-air
* http://airbreizh.asso.fr/le-projet-ambassadair/
* http://www.wiki-rennes.fr/Les_capteurs_Ambassad%27Air
* https://blog.adafruit.com/2018/12/17/biohack-know-your-air-quality/

## 18eme

* https://www.mairie18.paris.fr/actualites/dossier-notre-18e-durable-580
* http://28rueaffre.eklablog.com/le-bruit-et-l-odeur-a113885930  


