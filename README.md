# bareBones. Lo necesario para desarrollar código.
Muestra la arquitectura por capas de software. 
Presenta una arquitectura Modelo-Vista-Controlador en un archivo 
con dos tecnologías de sortware Php-HTML.

# Descripción.
Recupera registros-atributos de una tabla (libros) desde una 
base de datos (mvc), contenida en un archivo (libros.sql).

La _capa modelo_ tiene la responsabilidad de gestionar un 
objeto tipo mysqli **$consulta**, para vincular los todos los registros 
de la tabla libros. 
Mientras que la _capa controlador_  a través, de un objeto-interfaz 
**$filas** se serializan los atributos de cada registro y 
se acceden bajo la forma de un arreglo asosciativo por el espacio de 
memoria **$registros**.    

En la _capa vista_ se recuperan iterativamente los _tres elementos_ del 
arreglo asociativo **$atributos** en un elemento HTML tipo lista 
ordenada para ser renderizados en la interface del usuario.
  
	
