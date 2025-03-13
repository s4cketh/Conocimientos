Empezando con esto ![[Pasted image 20250312153815.png]]
vemos que el directorio no podemos borrarlo ya que hay un archivo con un sticky bit de pepe
pero si podremos borrarlo siendo root
![[Pasted image 20250312153941.png]]


EMPEZAMOS
Creamos una copia en una carpeta prueba
![[Pasted image 20250312154125.png]]

como bien sabemos podemos borrar estos archivos pero si lo hacemos podria ser grave y el equipo pierda muchas capacidades
 ![[Pasted image 20250312154241.png]]
entendiendo estos conceptos ahora veremos el 

lsattr
![[Pasted image 20250312154405.png]]
como vemos que es una copia le asignamos una flag especial
ahora le asignamos un
chattr  
+i    de inmutable
-V   nos muestra lo que pasa por atras cuando ejecutamos un comando
![[Pasted image 20250312154523.png]]

ahora intentamos borrar el archivo siendo root
![[Pasted image 20250312154723.png]]
vemos que no nos deja
porque?

como vemos aqui tiene una i de inmutable
![[Pasted image 20250312155222.png]]

![[Pasted image 20250312155303.png]]
y si le hacemos un chattr -i -V prueba
se quita




ADD
[chattr y lsattr: control de atributos de ficheros en Linux | rm-rf.es](https://rm-rf.es/chattr-y-lsattr-visualizar-y-modificar-atributos-en-sistemas-de-ficheros-linux/)
[Comandos Chattr y lsattr en Linux - programador clic](https://programmerclick.com/article/5604675172/)