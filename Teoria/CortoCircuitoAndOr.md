

# Operadores AND Y OR corto circuito

![tabla](/imagenesjava/tabladeverdad.png "tabla")






Anteriormente mencionamos los operadores AND y OR corto circuito. Lo que significa es que si se
detecta que el resultado ya no tiene sentido evaluarlo, por ejemplo si el operador && la
evaluación del operando del lado izquierdo es falso, ya sea como en este caso
entonces toda la evaluacion de aplicar la operacion AND, el unico valor posible del resultado de la operacion
sera falso, por lo tanto en este caso ya no tiene caso evaluar, el operador y , ya que sabemos
de antemano que el resultado de la operacion, sera falso.



![tabla1](/imagenesjava/tabladeverdad1.png "tabla1")



 Y en el caso del operador || si el operando del lado izquierdo
entonces el resultado es verdadero y por lo tanto ya no se evalúa el otro operando del lado
derecho, entonces si es verdadero el lado izquierdo, en automatico el resultado sera verdadero
y por lo tanto ya no se tendra que evaluar el lado derecho.

por eso se conocen como operadores de corto circuito, como el operador and y el operador or
tienen esta caracteristica.


