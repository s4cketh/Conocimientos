 Creamos nuestro directorio y cambiamos de propietario y grupo y damos permisos para que todos puedan **ESCRIBIR LEER EJECUTAR**
 ![[Pasted image 20250312150244.png]]
Ahora ingresamos a la directorio creado como pepe y creamos un txt 
![[Pasted image 20250312150454.png]]

nos volvemos kali ingresamos a la carpeta e intentamos eliminar el archivo creado por **pepe**
![[Pasted image 20250312150726.png]]
y nos deja borrar el archivo que creo pepe cuando no tenemos permiso de hacer eso, y ahora decimos que rayos? 
ahora volvemos atras para ver los permisos del directorio
![[Pasted image 20250312150850.png]]
aqui vemos que **otros** pueden alterar  y manipular todo

Y ahora como podemos evitar que otros no no puedan manipular un archivo que otro haya creado
![[Pasted image 20250312151154.png]]
le agregamos +t que es el sticky bit 

Ahora volvemos como kali vemos que podemos leerlo pero no podemos borrarlo y eso es la funcion del sticky bit
![[Pasted image 20250312151408.png]]





ADDDDDD
[Sticky Bit: ¿Qué es y cómo configurarlo? [2025] ](https://keepcoding.io/blog/que-es-el-sticky-bit-y-como-configurarlo/)
[El bit Sticky | Tutorial de GNU/Linux](https://www.fpgenred.es/GNU-Linux/el_bit_sticky.html)