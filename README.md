You will find the English ReadMe at the end of the document.

# Calliope mini CO₂-Sensor-Bibliothek, basierend auf der Sensirion SCD40 Makecode-Erweiterung

Makecode-Erweiterung für den Calliope mini CO₂-Sensor (SCD40), der mit der Calliope mini-Plattform verbunden ist.

Diese Erweiterung ermöglicht es, CO₂-, Temperatur- und relative Luftfeuchtigkeitswerte in einem Intervall von 5 Sekunden auszulesen.

## I2C-Adresse

* 0x62

## Verwendung

Öffne dein Calliope mini Makecode-Projekt. Gehe zu **„+ Erweiterung“** und füge die folgende URL ein:

https://github.com/calliope-edu/CO2-Sensor-SCD40

## API

CO₂-Wert in ppm abrufen
```ts
function get_co2()
```

Temperatur in Grad Celsius abrufen. Optionales Argument zum Umschalten auf Fahrenheit möglich.
```ts
function get_temperature()
```

Relative Luftfeuchtigkeit in Prozent ermitteln
```ts
function get_relative_humidity()
```

Messung starten. Diese Methode wird automatisch bei der Initialisierung aufgerufen.
Wenn du stop_continuous_measurement() aufgerufen hast, musst du diese Methode erneut aufrufen, bevor wieder CO₂-, Temperatur- oder Feuchtigkeitswerte ausgelesen werden können.
```ts
function start_continuous_measurement()
```

Messung beenden. Nach dem Aufruf dieser Funktion können keine Sensordaten mehr ausgelesen werden, bis start_continuous_measurement() erneut aufgerufen wird.
```ts
function stop_continuous_measurement()
```

## Hardware

![](icon.png)

## Supported Targets

* Calliopemini

## License

[MIT](LICENSE)


# Calliope mini CO2 Sensor library, based on Sensirion SCD40 MakeCode Extension

MakeCode extension for the Calliope mini CO2 Sensor (SCD40) connected to the Calliope mini platform.

This extension allows you to read CO2, temperature and relative humidity values with an interval of 5 seconds.


## I2C Address

* 0x62

## Usage

open your Calliope mini MakeCode project, in "+ Extension", paste the following URL:

https://github.com/calliope-edu/CO2-Sensor-SCD40


## API

Get CO2 value in ppm
```ts
function get_co2()
```

Get temperature in degree celsius. Takes an optional argument to change to fahrenheit.
```ts
function get_temperature()
```

Get relative humidity in percent
```ts
function get_relative_humidity()
```

Start measurement. This method will be automatically called on initialization.
If you call `stop_continuous_measurement()` you have to call this method again before CO2, temperature and humidity
values can be retrieved again.
```ts
function start_continuous_measurement()
```

Stop measurement. After calling this function, no more sensor values can be read out
anymore until you call `start_continuous_measurement`
```ts
function stop_continuous_measurement()
```

## Hardware

![](icon.png)

## Supported Targets

* Calliopemini

## License

[MIT](LICENSE)

Copyright (c) 2021, Sensirion AG
