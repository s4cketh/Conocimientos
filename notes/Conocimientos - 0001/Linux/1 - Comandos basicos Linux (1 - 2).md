Para ser un crack de cracks [La Chuleta de Comandos de Linux Definitiva](https://ciberninjas.com/chuleta-comandos-linux/)

**whoami** para saber que usuario eres
**id** ver a que grupos pertenecemos                       ![[Pasted image 20250311101651.png]]
en este caso vemos que pertenecemos a los grupos 
`adm, cdrom, floppy, sudo, audio, dip, video, pugdev, users, netdev, bluetooth, scanner, lpadmin, wireshark, kaboxer, vboxsf`

Cuando hacemos pentesting y cuando vulneramos alguna vulnerabilidad es bueno ver a que grupo pertenecemos ya que hay algunos usuarios con privilegios muy altos y asi seria fácil de comprometer el sistema

Con este comando listamos todo los grupos
`cat` listar el contenido de un archivo
`etc`  es un directorio
`group` un archivo
![[Pasted image 20250311104031.png]]

Filtrar por un nombre
`grep` filtrar 
`|` la barra sirve para decir que quiero usar otro comando en la misma linea
![[Pasted image 20250311105628.png]]