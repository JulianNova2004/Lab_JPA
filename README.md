# Laboratorio JPA

Este repositorio cuenta con el desarrollo del laboratorio de JPA

### Explicación de extensión

Para crear una relación de "uno a muchos" entre la entidad **Competitor** y el conjunto de **Producto**, se debe agregar la anotación _`@OneToMany`_ en la entidad **Competitor**. Esto indica que un competidor puede estar vinculado a varios productos. En la base de datos, este vínculo se refleja con una columna adicional en la tabla **Producto**, que actúa como clave foránea, apuntando al identificador del competidor. 

Además, el atributo _`mappedBy`_ se utiliza para especificar que la gestión de la relación se realiza desde la entidad **Producto**. De esta forma, la relación solo se refleja en la clave foránea de la tabla **Producto**, lo que ayuda a mantener la integridad referencial y asegura que las operaciones en cascada se apliquen de manera adecuada.


