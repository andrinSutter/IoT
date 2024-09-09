# Beispiel

Das Relay wird ein oder ausgestalten je nach dem welcher Knopf gedrückt wird und es wird auf das OLED Display geschrieben. 

Um zu testen ob das ganze funktioniert leuchtet eine kleine LED rot wenn das Relay an ist.

**Anschlus**: J7 P1

![image_11.png](image_11.png)

````Javascript
input.onButtonPressed(Button.A, function () {
    OLED.clear()
    OLED.writeStringNewLine("Relay ON")
    smartfeldAktoren.relaisEin(DigitalPin.P1)
})
input.onButtonPressed(Button.B, function () {
    OLED.clear()
    OLED.writeStringNewLine("Relay OFF")
    smartfeldAktoren.relaisAus(DigitalPin.P1)
})
OLED.init(128, 64)
````