---
comments: true
date: 2011-09-17 10:33:26
layout: post
slug: las-dos-vas
title: Las dos vías
wordpress_id: 476
categories:
- Filosofía
- misterios
- Mitos
tags:
- China
- doble
- dualidad
- filosofía
- Lao Tse
- misterios
- origen
- tao
- yang
- yin
---

> El Tao que puede ser expresado no es el Tao eterno.
El nombre que puede ser nombrado no es el nombre eterno.
Sin nombre, es principio del cielo y de la tierra, y con nombre, la Madre de los diez mil seres.
El que carece de deseos puede distinguir las esencias secretas.
Sin desprendernos del deseo, sólo vemos reflejos.
-- Tao Te Ching, citado por Joseph Campbell en Las Máscaras de Dios, Mitología Oriental.


La palabra Tao significa camino, la vía, la palabra Tê es la virtud o poder y Ching (king) es libro. Tao Te Ching es el libro del camino  del poder o la virtud (atenti Machiavelli). El tao chino es análogo al dharma hindú en tanto denota la verdad, la ley u orden del universo. En japonés es el D**ō.**

![Tao](/images/2011/09/Tao_thumb.png)

El Tao es el camino, la vía, y por tanto el método, la doctrina, la forma como se hace algo. El sinograma, el carácter han que lo representa se compone de dos partes: 首 (shǒu, que significa cabeza) y 辶(chuò que significa ir).

Hay muchas vías o caminos, el camino del hombre Ren Tao, que significa entre otras cosas procreación, se dice "que “los eunucos están muy lejos del Camino del Hombre”, está el camino del rey, que es gobernar, el Chu Tao, el Camino del Rey.

El Tao así con mayúsculas, el Dharma de los indios, ese camino del que habla Lao Tse (老子) está más allá de toda descripción. Su lado citerior, lo que está acá es la madre generadora de todas la cosas. Una cosa curiosa es que Lao Tse es un título honorífico, significa anciano erudito, no sabemos como se llamaba con certeza, para algunos era Li Er, para otros Boyang.

El taijitu, o símbolo tradicional del Tao es la representación tradicional del Taiji, o la dualidad del Yin y el Yang.

![El Yin y el Yang](/images/2011/09/yin-yang_thumb.png)

El diagrama simbólico del Tao representa los dos principios mediante una reciprocidad geométrica muy interesante como veremos en un momento.


> “El yang es el principio activo, claro, masculino,  caliente, seco, benéfico y positivo; el yin es su opuesto, pasivo,  oscuro, femenino, frío, húmedo, maligno, negativo. Cada parte ocupa la mitad de un círculo que representa el momento (eterno) en que se generaron los diez mil seres.

La línea divisoria de esta figura […] que ondula como una serpiente a lo largo del diámetro se compone de dos semicircunferencias cuyos diámetros equivalen a la mitad del diámetro de la circunferencia grande. Por tanto esta línea equivale a una semicircunferencia. El contorno del yin, como el del yang, es igual al contorno que rodea a ambos. Y si en vez de la línea divisoria, se traza una línea compuesta de cuatro semicircunferencias cuyos diámetros sean de nuevo la mita de largos, estos equivaldrían a una semicircunferencia del círculo principal. El resultado siempre será el mismo si se continúa la operación,  y la línea ondulante se aproximará al diámetro y tenderá a fundirse con éste. Finalmente se fundirán…” [1]


Vamos a explicar esto, es geometría simple, de esa que aprendimos en la escuela básica, no se asusten, pero es importante porque revela la belleza de esta símbolo para expresar este principio de la dualidad

Primero dibujas[2] un círculo de radio r, luego en la mitad superior dibujas un círculo de radio r/2, haces lo mismo en la parte inferior, como se ve en la figura:

![construccion-yin-yang](/images/2011/09/construccion-yin-yang_thumb.png)


Borras las mitades que están en gris con línea punteada y tendrás la figura básica, pintas de negro la parte inferior y obtienes el yin y el yang.


![yang](/images/2011/09/yang_thumb.png)


Ahora viene lo interesante, calculemos el perímetro del yang, la pare derecha es la mitad de la circunferencia grande grande ese valor es **π·r**, las otras mitades tienen un perímetro de **π·r/2**, si sumamos **π·r+2·(π·r/2) **obtenemos el perímetro del yang: **2·π·r**, que es el valor de la circunferencia que los contiene. Pasa lo mismo con el yin.

Es decir, si tienen una cuerda que cubra el borde del yin, otra que cubra el borde del yang, ambas tendrán el mismo largo que la cuerda que cubra al circulo que las envuelve.

El yin y el yang tienen la misma superficie, pero si los deformamos pueden alcanzar la forma del círculo completo.




> “Lo que este diagrama representa geométricamente es el misterio de una circunferencia que se convierte en dos y, de esta forma, produce los diez mil seres de la creación. Por otra parte, el aspecto ulterior, inefable, del mismo misterio, se representa simplemente con un círculo.

El yin y el yang, están presentes en todas las cosas. Son inseparables y no se les puede juzgar moralmente como bueno o malo. Actúan juntos en una interacción perpetua en la que cada vez predomina uno. En el hombre predomina el yang, en la mujer el yin, pero los dos están presentes en ambos.” [1]


Esta es la dualidad de la filosofía oriental. En la biblia es Eva que surge de Adán, en el pensamiento cristiano occidental tenemos la imagen del uno que se hace dos (recuérdese el relato del hermafrodita en el Banquete de Platón). “El símbolo del tao puede ser una imagen de la condición dual de Adán antes de que Eva fuera separa de él. No obstante, a diferencia de de la figura bíblica y análogamente a la imagen india del Yo que se dividió en dos, el tao es inmanente, además de trascendente: es la esencia secreta de todas las cosas y, sin embargo, su misterio más profundo.”

Dice el Tao Te King:


> “En su origen, son el mismo, pero sus nombres son diferentes;
Al origen le llamamos el Gran Misterio:
Y del Misterio, el Misterio más oscuro aún es el portal de todas las esencias secretas.”


## Notas:

[1] Joseph Campbell, Las Máscaras de Dios Volumen 2. ISBN 978-84-206-9622-5

[2] El siguiente programa en python permite dibujar el yin y el yang, lo que permite apreciar mejor su geometría:

```python
    from turtle import *

    def yu(radio, color1, color2):
		width(3)
		color("black")
		begin_fill()
		circle(radio/2, 180)
		circle(radio, 180)
		left(180)
		circle(-radio/2, 180)
		color(color1)
		end_fill()
		begin_fill()
		color(color2)
		left(90)
		up()
		forward(3*radio/8)
		right(90)
		down()
		circle(radio/8)
		left(90)
		end_fill()
		up()
		backward(3*radio/8)
		down()
		left(90)

    yu(200, "white", "black")
    yu(200, "black", "white")
    ht()
    mainloop()
```
