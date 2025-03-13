Considerando un binario
![[Pasted image 20250312155854.png]]
vemos su ruta absoluta
nuevo comando **xargs**
**xargs** sirve para usar otro comando ma
![[Pasted image 20250312160206.png]]
aqui vemos que tiene el permiso **755**

Asignando privilegio SUID
![[Pasted image 20250312160329.png]]

Abrimos otra terminal y vemos que hay un archiuvo con privilegios SUID
![[Pasted image 20250312160438.png]]

s =4000

busqueda de SUID desde la raiz
![[Pasted image 20250312160709.png]]

Ahora sabiendo que existen archivos con permisos SUID debemos saber que siendo el usuario que seamos podemos ejecutar ese archivo de forma temporal como el propietario ya que tiene permisos SUID

![[Pasted image 20250312161026.png]] ![[Pasted image 20250312161113.png]]



Ver binarios que se estan ejecutando con el grupo root
![[Pasted image 20250312161250.png]]



![[Pasted image 20250312161707.png]]
seria 4755
![[Pasted image 20250312161728.png]]
2755




[Permisos SGID, SUID y Sticky Bit - Linux - Deep Hacking](https://deephacking.tech/permisos-sgid-suid-y-sticky-bit-linux/#:~:text=Permiso%20SGID,-El%20permiso%20SGID&text=Si%20se%20establece%20en%20un,perteneciente%2C%20el%20grupo%20del%20directorio.)
[Permisos especiales en Linux: Sticky Bit, SUID y SGID - ochobitshacenunbyte](https://www.ochobitshacenunbyte.com/2019/06/17/permisos-especiales-en-linux-sticky-bit-suid-y-sgid/)
[Los bits SUID, SGID y sticky](https://www.ibiblio.org/pub/linux/docs/LuCaS/Manuales-LuCAS/SEGUNIX/unixsec-2.1-html/node56.html)