

`````` java

//los valores se evaluan de izquierda a derecha.

 public static void main(String[] args) {
        //Declaracion de 3 variables el cual se les asignan valores a cada uno.
        var x = 5;
        var y = 10;
        var z = ++x + y--; //se evaluaron los operadores unarios (++ y --) y finalmente se evaluo la suma.

        System.out.println("x = " + x); //6
        System.out.println("y = " + y); //9
        System.out.println("z = " + z); //16
        
        var resultado = 4 + 5 * 6 / 3;//4 + ((5*6)/3) -> 4 + (30/3) -> 4 + 10 , por prioridad se realiza primero lo que esta dentro del parentesis, luego la division y de ultimo la suma.
        System.out.println("resultado = " + resultado);
    
        resultado = (4 + 5) * 6/3; //-> (9 * 6)/3 -> 54/3, se suma lo que esta dentro del parentesis, despues se hace la division y de ultimo se hace la multiplicacion.
        System.out.println("resultado = " + resultado);
    }


`````` 