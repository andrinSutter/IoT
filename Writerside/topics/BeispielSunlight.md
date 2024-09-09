# Beispiel


**Anschluss:** J5

![image_13.png](image_13.png)

````Javascript
smartfeldSensoren.initSunlight()
OLED.init(128, 64)
loops.everyInterval(500, function () {
    OLED.clear()
    OLED.writeStringNewLine("Licht: " + smartfeldSensoren.getHalfWord_Visible())
    OLED.writeStringNewLine("IR: " + smartfeldSensoren.getHalfWordIR())
})
loops.everyInterval(5000, function () {
    if (100 <= smartfeldSensoren.getHalfWord_Visible()) {
        music._playDefaultBackground(music.builtInPlayableMelody(Melodies.PowerUp), music.PlaybackMode.UntilDone)
    }
})

````