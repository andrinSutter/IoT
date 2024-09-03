# Beispiel

Ich habe hier einen kleinen Code der den Abstand zu verschiedenen Objekten oder Hindernissen messen kann.

**Anschluss:** J1
![image_1.png](image_1.png)

`````Javascript
OLED.init(128, 64)
OLED.clear()
loops.everyInterval(500, function () {
    OLED.clear()
    OLED.writeString("" + Math.round(smartfeldSensoren.measureInCentimetersV2(DigitalPin.P0)) + "cm")
})
`````