Creamos un archivo .sh y le damos permisos de ejecucion

![[Pasted image 20250312193301.png]]
abrimos nuestro archivo con vim
**vim scrip.sh**

![[Pasted image 20250312193525.png]]
GUARDAR Y SALIR
![[Pasted image 20250312193634.png]]
precionamos esc luego ponemos el siguiente comando 
guardamos con  :wp



EJECUTAMOS
![[Pasted image 20250312193721.png]]


AHORA
![[Pasted image 20250312194134.png]]
no quedamos con el eth0 porque ahi se encuentra nuestra ip
![[Pasted image 20250312194212.png]]
ahora le decimos que nos quedaremos con la ultima linea

![[Pasted image 20250312194423.png]]
otra forma seria con awk 
![[Pasted image 20250312194613.png]]
Ahora el 2do argumento
![[Pasted image 20250312194742.png]]
Ahora le decimos quiero que me des el primer argumento tomando de delimitador la /
![[Pasted image 20250312194916.png]]
otra forma
seria 
quiere decir como delimitador la / pues quiero quedarme con el primer campo `-f 1`
![[Pasted image 20250312195002.png]]

tambien podemos decirle que convierta las / en espacios y que use el primer dato
![[Pasted image 20250312200244.png]]

Ahora agregamos el codigo que gustemos
![[Pasted image 20250312200553.png]]
luego ejecutamos
![[Pasted image 20250312200655.png]]
agregamos saltos de linea
-e es para que nos detecte los caracteres especiales que agregamos como \n
![[Pasted image 20250312200820.png]]
ejecutamos
![[Pasted image 20250312200830.png]]
