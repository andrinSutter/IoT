# Capacitive Moisture Sensor

Der **Capacitive Moisture Sensor** ist ein Sensor, welcher die Feuchtigkeit im Boden misst. Hier ist eine einfache Erklärung:

- **Wie es funktioniert**: Der Sensor nutzt elektrische Kapazitätsänderungen, die durch die Feuchtigkeit im Boden verursacht werden.
- **Messung**: Ein change in Bodenfeuchtigkeit ändert die Kapazität des Sensors, was dann in ein digitales Signal umgewandelt wird.
- **Verwendung**: Oft benutzt in Gartenbau, Landwirtschaft und automatischer Bewässerung.
- **[Beispiel Anwendung](BeispielCMS.md)**: Man könnte daraus eine automatische Bewässerung bauen, indem der Feuchtigkeitssensor die Erde misst und wenn es unter einen bestimmten Wert fällt wird eine Bewässerungsanlage gestartet. 

## Specification

| Item                | Value          |
|---------------------|----------------|
| Operating Voltage   | 3.3V / 5V      |
| Output Interface    | Analog         |

## Ports

Am besten nimmt man **J1-J3** da wir ein Analoges Signal haben. J0 und J5 funktionieren nicht da wir keinen P Port haben

Zusammengefasst: Der Sensor misst die Bodenfeuchtigkeit, indem er Änderungen in der elektrischen Kapazität erkennt.
