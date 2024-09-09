# Sunlight Sensor

Der **Sunlight Sensor** ist ein Sensor, welcher die Intensität des Sonnenlichts misst. Hier ist eine einfache Erklärung:

- **Wie es funktioniert**:
    - Der Sensor verwendet Fotozellen, die Licht in elektrische Signale umwandeln.
    - Er misst verschiedene Lichtwellenlängen, darunter Infrarot, sichtbares und ultraviolettes Licht.
- **Messung**: Erfasst die Helligkeit und spektrale Zusammensetzung des Sonnenlichts.
- **Verwendung**: Oft benutzt in Solarenergie-Systemen, Umweltüberwachung und zur Anpassung der Beleuchtung in Gebäuden.
- **[Beispiel Anwendung](BeispielSunlight.md)**: Man könnte einen Wecker, welcher mit Sonnenlicht gesteurt ist bauen. Wenn der Lichtwert eine bestimmte Grenze erreicht wird ein Wecker Ton abgespielt.

## Specification

|||
|------------------------|---------------|
| Operating Voltage      | 3.0-5.5V      |
| Working Current        | 3.5mA         |
| Wave Length            | 280-950nm     |
| Default I2C Address    | 0x60          |
| Operating Temperature  | -45-85℃       |

## Ports

Der Sunlight Sensor besitzt einen I2C Interface(7-bit) deshalb benutzen wir den Port **J5**

Zusammengefasst: Der Sunlight Sensor misst die Lichtintensität und spektrale Zusammensetzung des Sonnenlichts und gibt entsprechende elektrische Signale aus.
