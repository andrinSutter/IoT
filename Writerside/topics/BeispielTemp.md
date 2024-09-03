# Beispiel

In diesem Beispiel werden verschiedene Luftdaten auf den OLED Screen geschrieben.

**Anschluss:** J5

![image_3.png](image_3.png)

````Javascript
smartfeldSensoren.gas_init()
OLED.init(128, 64)
OLED.clear()
loops.everyInterval(500, function () {
    OLED.clear()
    OLED.writeStringNewLine("Luft: " + smartfeldSensoren.readGasHum())
    OLED.writeStringNewLine("Temp:  " + smartfeldSensoren.readGasTemp())
    OLED.writeStringNewLine("CO2: " + smartfeldSensoren.readGasCO2eq())
})
````