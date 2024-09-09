# Beispiel

**Anschluss**: J3 (P2)

![image_12.png](image_12.png)

````Javascript
OLED.init(128, 64)
OLED.clear()
loops.everyInterval(500, function () {
    OLED.clear()
    OLED.writeStringNewLine("Feuchtigkeit: " + smartfeldSensoren.bodenfeuchteGibFeuchte(AnalogPin.P2))
})
loops.everyInterval(5000, function () {
    if (500 >= smartfeldSensoren.bodenfeuchteGibFeuchte(AnalogPin.P2)) {
        OLED.writeStringNewLine("bewässern")
        music._playDefaultBackground(music.builtInPlayableMelody(Melodies.Wawawawaa), music.PlaybackMode.InBackground)
    }
})

````