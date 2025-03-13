

------
`Creacion de usuario`
creamos un directorio **pep** siendo root
![[Pasted image 20250312102631.png]]


`creacion de usuario`
![[Pasted image 20250312103205.png]]
agregar usuario **useradd  pepe**
para asignarle una bash **-s /bin/bash**
para darle un directorio personal de usuario **-d /home/pep**



`Verificacion de la creacion`
![[Pasted image 20250312103237.png]]
Vemos que  que el identificador es el 1001
Vemos que su home asignado y tambien la shell que le dimos


`Verificacion de grupo`
![[Pasted image 20250312103339.png]]
Vemos que el identificador de su grupo es 1001


`Asignacion de contraseña`
![[Pasted image 20250312103614.png]]

Vemos que el propietario y el grupo son root
![[Pasted image 20250312103705.png]]


`Cambio de grupo`
![[Pasted image 20250312103835.png]]
**chgrp pepe pep**  basicamente significa en español
pepe quiero asignar como grupo al directorio pep

``Cambio de propietario`
![[Pasted image 20250312104241.png]]


/////////MATANDO 2 PAJAROS DE UN TIRO////////////
![[Pasted image 20250312104428.png]]
el 1er pepe es para el propietario
el 2do pepe es grupo
y pep el directorio
en español  
quiero asisgnar de propietario a pepe : grupo a pepe en el directorio pep
////////////////////



`Verificacion`
![[Pasted image 20250312104629.png]]



`Agregar usuario a un grupo en especifico`
creamos grupo
![[Pasted image 20250312104824.png]]
agregamos al usuario pepe parte del grupo Alumnos 
![[Pasted image 20250312104846.png]]
`verificacion de que migramos al grupo Alumnos`
![[Pasted image 20250312104944.png]]


`EJERCICIO "PRACTICANDO"`
![[Pasted image 20250312105253.png]]  ![[Pasted image 20250312105337.png]]


Para cacharrear    **volverte un crag**
[Gestionar Usuarios, Grupos y Permisos en Linux ](https://computernewage.com/2016/05/22/gestionar-usuarios-y-permisos-en-linux/)
[Gestión de usuarios y grupos en Linux ](https://atareao.es/como/gestion-de-usuarios-y-grupos-en-linux/)
