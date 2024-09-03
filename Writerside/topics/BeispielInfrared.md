# Beispiel

In diesem Beispiel wird eine 1 bei erkenntem Objekt/Hinderniss angezeigt und eine 0 bei nichts erkanntem.

**Anschluss:** J6

![image_4.png](image_4.png)

````Javascript
loops.everyInterval(500, function () {
    basic.showString("" + (smartfeldSensoren.reflectiveLightsensorObjectDetected(DigitalPin.P14)))
})
````