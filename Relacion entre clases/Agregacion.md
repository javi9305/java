## Agregación  



Imaginemos una clase celular y una clase chip, cuando un celular se crea, no tiene ningun chip, pero con el tiempo le podemos agregar 1 o hasta 2 chips, en cualquier caso el celular seguira funcionando,esto es porque el chip no es parte del celular, solamente esta dentro del celular, es decir la clase celular y la clase chip pueden funcionar uno independientemente del otro.

![celular](/imagenesjava/celular1.png)  


![celular](/imagenesjava/celular2.png)

En esta relacion podemos identificar 2 roles la clase contenedor y la clase elemento.

![celular](/imagenesjava/celular3.png) 




una regla importante de agregacion es que si la clase contenedora es destruida, los elementos deberan seguir existiendo.


![celular](/imagenesjava/celular4.png) 




el diagrama de la clase se veria asi:  

![celular](/imagenesjava/celular5.png) 


el simbolo que indica la agregacion es esa linea con un rombo vacio apuntando a la clase contenedora en este caso celular, esta relacion se leeria como "tiene" o "Esta en"  es decir un celular tiene un chip o un chip esta en un celular.  

tambien debemos tomar en cuenta la cardinalidad nos da una mejor idea de como funciona esta relacion, en este caso la cardinalidad es de 1 a n, ya que un celular puede tener varios chips, pero un chip solo puede estar en un celular.