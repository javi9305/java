# Operador de composición de suma

![operador](/imagenesjava/operadorcomposicion.png "operador")


Tambien puede aplicarse para resta, multiplicación y división

# Operadores relacionales

Los operadores relacionales nos permiten hacer una comparación entre dos valores y determinar un resultado de tipo Booleano (true o false).

Ejemplos

        10 < 3 = false
        4 == 4 = true
        En los char se compara con los valores Unicode (ya que son numéricos).
         a < b 

# Operadores lógicos/condicionales

trabajan con operadores booleanos


        AND         &&

         OR          ||   

         NOT          !   
  
         OR           | 

         AND          &

         XOR          ^

Ejemplos: 

Cuando ambos(X o Y) sean verdaderos

   boolean x = true;
   boolean y = false;

**Tabla de verdad AND(&&)**

|             |              |      
|   ----------|:------------:|
|  x && x     |    true 
|  x && y     |    false      
|  y && x     |    false       
|  y && y     |    false


Algunos de los dos(X o Y) sea verdadero.

boolean x = true;

boolean y = false;

**Tabla de verdad Or (||)**


  x || x         true 

  x || y         true  

  y || x         true  

  y || y         false




**Lo contrario de (X o Y).**

boolean x = true;

boolean y = false;

**Tabla de verdad Not (!)**

|             |              |      
|   ----------|:------------:|
|    ! y      |    true 
|    ! x      |    false

Ambos diferentes  (X o Y) para que el resultado sea true.

boolean x = true;

boolean y = false;

**Tabla de verdad XOr (| |)**

|             |              |      
|   ----------|:------------:|
|   x ^ x     |    false
|   x ^ y     |    true      
|   y ^ x     |    true       
|   y ^ y     |    false


¿Cuál es la diferencia entre && y &   o   || y | ?

La diferencia está en la forma de evaluación 

&& y || se evalúan en corto circuito.

& y |  se evalúan ambos operandos.

Ejemplo

Int x = 0;

Int y = 2;

                   Ambos deben ser true.

 Boolean b = (x!=0) && ((y/x)!=0) =  false (devuelve false  porque hace corto circuito  ya que no evalúa el segundo paréntesis  debido al que el  primer paréntesis dio false, 
 
 ya que ambos deben ser verdaderos ).


Boolean b = (x!=0) &  ((y/x)!=0);

Evalúa forzosamente los dos componentes pero en este caso mandaría lo que es una excepción y ya no arrojaría ningún resultado.

**nota:** cuando usamos el true en un if por ejemplo

if(valorBoleano == true)

podemos abreviarlo asi:

if(valorBoleano)


# Operaciones con cadenas de caracteres.

Los Strings son objetos los cuales tiene métodos que se encuentran en la documentación del api de java la cual es: [](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html.)

La concatenación es unir dos o más Strings. 

Acciones que se pueden realizar con un String:

*	Unir o concatenar(es unir dos o más String)
*	Contar su tamaño
*	Extraer una porción de esa cadena
*	Comparar dos cadenas.
*	Reemplazar un carácter.
*	Quitar los espacios en blanco.
*	Convertir sus caracteres a mayúscula.
*	Convertir sus caracteres en minúscula.

La siguiente instrucción permite la lectura de datos desde el teclado:

`````` java
           Scanner sc = new Scanner(System.in);
           Int variable= sc.nextInt ();
``````           

          El objeto scanner permite mediante su método nextInt, obtener datos
          enteros desde teclado.

# Precedencia de operadores

![precedencia](/imagenesjava/precedencia.png "precedencia")

![precedencia2](/imagenesjava/precedencia2.png "precedencia2")


La precedencia es de izquierda a derecha.

Ejemplo:

12/3 + 2 * 2- 1 =

4 + 2 * 2 – 1  = 

4 + 4 -1 = 7 
