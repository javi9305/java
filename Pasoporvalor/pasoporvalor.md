
`````` java

 public static void main(String[] args) {
       var x = 10; //va a ser de tipo entero
       
       /*
       el paso de valor aplica a los tipos primitivos.
       */
        System.out.println("x = " + x);
       
       cambiarValor(x);
       
        System.out.println("x = " + x);
    } 

    //el metodo solo se puede usar dentro de esta clase.
    //si estamos dentro del main, los metodos deben de ser estaticos.
    //pasamos una copia del valor x a la variable arg.
    private static void cambiarValor(int arg) {  //int arg = 10, cuando mandamos a llamar el metodo cambiarValor(x)
        arg = 20;
        System.out.println("arg = " + arg); //al terminar el metodo cambiarValor, arg se destruye.
    }

    ``````