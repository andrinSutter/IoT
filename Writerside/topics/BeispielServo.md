# Beispiel

![image_14.png](image_14.png)

````Javascript
loops.everyInterval(1000, function () {
    smartfeldAktoren.set_angle(AnalogPin.P2, 180)
    basic.pause(500)
    smartfeldAktoren.set_angle(AnalogPin.P2, 0)
})
basic.forever(function () {
	
})
````