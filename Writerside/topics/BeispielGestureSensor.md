# Beispiel

In diesem Beispiel werden 4 Gesten erkannt und auf dem LED Screen ausgegeben.

**Anschluss:** J5

![image_2.png](image_2.png)

````Javascript
smartfeldSensoren.onGesture(GroveGesture.Left, function () {
    basic.showLeds(`
        . # . . .
        . . # . .
        . . . # .
        . . # . .
        . # . . .
        `)
})
smartfeldSensoren.onGesture(GroveGesture.Up, function () {
    basic.showLeds(`
        . . . . .
        . . # . .
        . # . # .
        # . . . #
        . . . . .
        `)
})
smartfeldSensoren.onGesture(GroveGesture.Down, function () {
    basic.showLeds(`
        . . . . .
        # . . . #
        . # . # .
        . . # . .
        . . . . .
        `)
})
smartfeldSensoren.onGesture(GroveGesture.Right, function () {
    basic.showLeds(`
        . . . # .
        . . # . .
        . # . . .
        . . # . .
        . . . # .
        `)
})
smartfeldSensoren.initGesture()

````