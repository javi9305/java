## Composición

Imagina un celular y una bateria, un celular no puede funcionar sin energia, es decir sin una bateria,ya que la clase bateria depende del celular.

![celular](/imagenesjava/celular6.png)

En la composicion podemos identificar 2 roles: la clase todo y la clase parte.

![celular](/imagenesjava/celular7.png)

una regla importante de la composicion, si un objeto todo es destruido, tambien seran destruidas sus partes.

![celular](/imagenesjava/celular8.png)

el diagrama de clases del ejemplo se veria asi:

![celular](/imagenesjava/celular9.png)

Para representar la composicion en el diagrama se usa una linea con un rombo pintado que apunta a la clase todo, en este caso celular, la relacion se leeria "Se compone de" o "Compone a" es decir un celular se compone de una bateria o una bateria compone a un celular.

La cardinalidad en este caso es de 1 a 1, ya que un celular se compone de una sola bateria y una bateria es parte de un solo celular.

