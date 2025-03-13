Creamos una carpeta con el super usuario root
luego denigramos a nuestro usuario kali
![[Pasted image 20250311200435.png]]
aqui podemos ver que tiene los permisos de
`drwxr-xr-x`
procedemos a separlos de a 3
d= directorio
rwx     r-x       r-x

como somos usuario savitar y vemos que propietario y grupo son root
Concluimos que somos otros, nuestros permisos serian `r-x`  osea tenemos capacidad de  lectura y atravesar el directorio pero no podremos crear contenido 

Aqui vemos que podemos entrar pero no podemos crear una carpeta ni directorio
![[Pasted image 20250311200902.png]]

**Editamos permisos**
`chmod` Sirve para dar permisos solo si tenemos permisos para hacerlo
en este caso tuve que ser root para darle permiso de editar a otros
![[Pasted image 20250311201131.png]]
otra forma 

Para asignarle un grupo 
![[Pasted image 20250311202518.png]]
Otra forma de cambiar permisos
![[Pasted image 20250311202946.png]]
![[Pasted image 20250311202958.png]]
![[Pasted image 20250311202930.png]]
 ***P*
 *A*
 *R*
 *A*
 *MAS* 
 *T*
 *I*
 *P*
 *S*
 [Propietarios y permisos - atareao con Linux](https://atareao.es/tutorial/terminal/propietarios-y-permisos/)
 