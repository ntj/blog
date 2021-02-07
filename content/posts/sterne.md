+++
title = "Sterne generieren"
date = 2021-02-06T20:06:45+01:00
images = []
tags = []
categories = []
draft = false
+++
Vor nicht allzu langer Zeit habe ich an Quellcode gebastelt, mit dem ich mir Sterne generieren kann, die den Papiersternen
ähneln, die man aus quadratischem Papier faltet.

Die Ecken des Quadrats werden diagonal übereinander gelegt. Das wiederholt man ein paar Mal, bis ein kleines Dreieck entsteht. Dann schneidet man ein paar Ecken in die Kanten des Dreiecks, faltet es wieder auseinander und erhält einen wunderschönen Stern, der an eine Schneeflocke erinnert.

Das ganze passiert jetzt in Quellcode mit vielen randomisierten Werten, so dass kein Stern dem anderen gleicht.

Hier sind die Ergebnisse:

![Stern](https://github.com/ntj/sandbox/blob/master/img/star2-1.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star2-2.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star2-3.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star2-4.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star2-5.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star2-6.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star2-7.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star2-8.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star2-9.svg?raw=true)


Der Quellcode ist auf [github](https://github.com/ntj/sandbox) veröffentlicht. Eine Stelle möchte ich erklären:

```python
{
  def point(a, b, c, x, y, z):
    px = a[0] * x + b[0] * y + c[0] * z
    py = a[1] * x + b[1] * y + c[1] * z
    return[px,py]
}
```
Hier verwende ich [baryzentrische Koordinaten](https://de.wikipedia.org/wiki/Baryzentrische_Koordinaten). Wenn die Koordinaten der Eckpunkte eines Dreiecks mit Faktoren multipliziert werden, die aufsummiert 1 ergeben, dann resultiert das
in einem Punkt, der sich immer innerhalb des Dreiecks befindet.

Um welches Dreieck geht es? Der Stern ergibt sich, weil ein rechtwinkliges Dreieck
an verschiedenen Achsen gespiegelt wird, horizontal, vertikal und diagonal.
So ähnlich wie beim Papierfalten schneide ich nun Ecken aus dem Dreieck heraus. Dafür
benötige ich die Punkte, die sich innerhalb des Sterns befinden.

So sieht das Ganze dann für die obigen Sterne aus:


![Polygon](https://github.com/ntj/sandbox/blob/master/img/polygon-1.svg?raw=true)
![Polygon](https://github.com/ntj/sandbox/blob/master/img/polygon-2.svg?raw=true)
![Polygon](https://github.com/ntj/sandbox/blob/master/img/polygon-3.svg?raw=true)
![Polygon](https://github.com/ntj/sandbox/blob/master/img/polygon-4.svg?raw=true)
![Polygon](https://github.com/ntj/sandbox/blob/master/img/polygon-5.svg?raw=true)
![Polygon](https://github.com/ntj/sandbox/blob/master/img/polygon-6.svg?raw=true)
![Polygon](https://github.com/ntj/sandbox/blob/master/img/polygon-7.svg?raw=true)
![Polygon](https://github.com/ntj/sandbox/blob/master/img/polygon-8.svg?raw=true)
![Polygon](https://github.com/ntj/sandbox/blob/master/img/polygon-9.svg?raw=true)



Die zusammengesetzten Sterne lassen sich bestimmt gut mit dem Lasercutter
ausschneiden -- für den nächsten Weihnachtsbaum.


![Stern](https://github.com/ntj/sandbox/blob/master/img/star1-1.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star1-2.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star1-3.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star1-4.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star1-5.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star1-6.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star1-7.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star1-8.svg?raw=true)
![Stern](https://github.com/ntj/sandbox/blob/master/img/star1-9.svg?raw=true)
