Para generar valores aleatorios en Java existe una clase llamada
**Random** en el paquete **java.util.Random.** Esta clase posee
metodos que te permiten obtener numeros pseudoaleatorios.

usaremos la tabla de caracteres **ASCII** y el metodo **nextInt()** de la claase Random para generar valores enteros
entre 0 y 9 para obtener los digitos y tambien entre 65 y 90 para obtener las letras a partir de la conversion de numeros
enteros a caracteres de la tabla ASCII.

Para utilizar la clase Random tenemos que importar primero
el paquete **java.util.Random** al comienzo de nuestro archivo
fuente.

`````` java
import java.util.Random.

``````



Luego podrás implementar esta parte código para almacenar como cadena de texto tu matrícula con valores aleatorios:

`````` java
// Inicializamos la variable que almacenará la matrícula.
String Matricula = "";
// Inicializamos la instancia de la clase Random con la que
// generaremos el valor aleatorio.
Random rnd = new Random();

// Creamos un ciclo que se ejecute 7 veces, que corresponden al
// texto de la matrícula.
for (int i = 0; i < 7; i++)
{
    // Con este condicional verificamos si estamos en la parte
    // numérica o alfabética de la matrícula.
    // Solo debe entrar al condicional si estamos generando los
    // números de la matrícula.
    if(i < 4)
    {
        // Con esta instrucción se genera un número aleatorio entre
        // 0 y 9, no se incluye el 10.
        Matricula += rnd.nextInt(10);
    }
    // Entrará en esta parte del condicional cuando estemos generando
    // las letras de la matrícula.
    else
    {
        // Con esta instrucción se genera un número aleatorio entre
        // 65 y 90, no se incluye el 91. Luego se convierte a un 
        // caracter ASCII.
        Matricula += (char)(rndnextInt(91) + 65);
    }
}

// Por último imprimimos la matrícula en la consola.
System.out.println("La matrícula es: " + Matricula);

``````


De manera en que así te quedaría el código que propongo para tu problema:


``````java
import java.util.Random;

public static void main(String[] args) 
{
    String Matricula = "";
    Random rnd = new Random();

    for (int i = 0; i < 7; i++)
    {
        if(i < 4)
        {
            Matricula += rnd.nextInt(10);
        }
        else
        {
            Matricula += (char)(rndnextInt(91) + 65);
        }
    }

    System.out.println("La matrícula es: " + Matricula);
}


``````

Si desearas que la parte alfabética de la matrícula generada aleatoriamente no contenga una serie de caracteres puedes usar el método indexOf() de la clase String en conjunto con un bucle while para comparar si el carácter generado se encuentra en la lista de letras que no deseas que aparezcan en tu matrícula y así no imprimirlo.

Para lograr eso, en conjunto con el método Random.nextInt(), te propongo el siguiente código:

``````java
import java.util.Random;

public static void main(String[] args) 
{
    char Caracter;
    String Matricula = "";
   // Aquí se definen las letras que no quieres que se generen.
    String CaracteresNoDeseados = "AEIOU";
    Random rnd = new Random();

    for (int i = 0; i < 7; i++)
    {
        if(i < 4)
        {
            Matricula += rnd.nextInt(10);
        }
        else
        {
                do 
            {
                Caracter = (char)(rndnextInt(91) + 65);
            // Si el carácter existe en la cadena de texto 
            // de los no deseados, se repite el bucle
            } while (CaracteresNoDeseados.indexOf(Character) >= 0)

            Matricula += Caracter;
        }
    }

    System.out.println("La matrícula es: " + Matricula);
}



``````


En esta guía que habla acerca de cómo generar números aleatorios con la clase Random. Encontrarás también que puedes generar un número aleatorio con la clase Math y su método random en esta página. Usar el método Math.random es válido también, así que podrías también intentar aplicarlo para tu solución.

Si deseas cambiar el uso del método Random.nextInt() por el método Math.random() debes eliminar la línea en donde se declara la variable rnd y cambiar las siguientes líneas de código:

Matricula += rnd.nextInt(10);

Por:

Matricula += (int) Math.floor(Math.round() * 10);

Y

Matricula += (char)(rndnextInt(91) + 65);

Por:

Matrícula += (char)((int) Math.floor(Math.round() * 91 + 65));