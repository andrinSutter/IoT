# Beispiel

Es wird ein Smiley angezeigt sobald der Schalter gedrückt wird.

**Anschluss:** J6

![image_6.png](image_6.png)

````Javascript
basic.forever(function () {
	
})
loops.everyInterval(100, function () {
    if (0 < smartfeldSensoren.microswitchActuated(DigitalPin.P0)) {
        basic.showLeds(`
            . # . # .
            . # . # .
            . . . . .
            # . . . #
            . # # # .
            `)
    } else {
        basic.showLeds(`
            . # . # .
            . # . # .
            . . . . .
            . # # # .
            # . . . #
            `)
    }
})
````