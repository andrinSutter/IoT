# Beispiel

Auf dem OLED Display werden die Lichtwerte angegeben.

**Anschluss:** J5

![image_8.png](image_8.png)

````Javascript
smartfeldSensoren.initSunlight()
OLED.init(128, 64)
loops.everyInterval(500, function () {
    OLED.clear()
    OLED.writeStringNewLine("Licht: " + smartfeldSensoren.getHalfWord_Visible())
    OLED.writeStringNewLine("IR: " + smartfeldSensoren.getHalfWordIR())
})
````