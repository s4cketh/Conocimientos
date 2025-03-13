`Concatenar comandos`
![[Pasted image 20250311113926.png]]

`Concatenar con` **&&**
El 2do operando solo se ejecuta si el primer operando es exitoso
![[Pasted image 20250311114104.png]]
` Y como sabemos si el comando es exitoso o no? Una vez realizado la operacion usamos ` **echo $?**
0 -> exitoso
otro numero -> No exitoso
![[Pasted image 20250311114425.png]]
`Para que se los 2 procesos continuen aunque haya error  ` **||** -> or
![[Pasted image 20250311114755.png]]
#### stedeer -> es el error

`Para usar comando y que no aparezca ese texto de error` redireccionamos al **2>/dev/null**
el 2>/dev/null es como un agujero negro como el tacho de basura
![[Pasted image 20250311115320.png]]
`Para convertir el stedount en un stedout ` **&>/dev/null  & disown**  -> se usa como por ejemplo para abrir wireshark sin que se muestre el output en la terminal
