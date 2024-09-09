# Beispiel

Der Potentiometer Wert wird auf den OLED Screen geschrieben.

**Anschluss:** J3

![image_7.png](image_7.png)

````Javascript
OLED.init(128, 64)
loops.everyInterval(500, function () {
    OLED.clear()
    OLED.writeStringNewLine("Potentiometer:" + smartfeldSensoren.potentiometerGibProzent(AnalogPin.P0, AnalogPin.P16))
})
````