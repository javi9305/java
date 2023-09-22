# Concatenación

Estos son datos asignados a variables.

var usuario    =       "Juan";                                         var i    =     3;                           var j   =    4;

Se evaluara dichos valores en 3 casos que son los siguientes:

1.	Evaluación de izquierda a derecha

System.out.println(**i + j + usuario**)

**Imprime: 7juan**

2.	Contexto cadena, todo es una cadena

System.out.println(**usuario + i + j**)

**Imprime: juan34**

3. Uso de paréntesis modifican la prioridad de la evaluación

System.out.println(**(usuario + (i + j))**)

**Imprime: juan7**