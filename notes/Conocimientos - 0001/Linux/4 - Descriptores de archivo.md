#bash
**exec 3 <> file** 

 `1. <  lectura
 `2. > escritura`
cod 1: nos creamos una arhivo file 
estamos empleando un descriptor de archivo con el nombre 3
![[Pasted image 20250311162114.png]]       
`Metemos el output de whoami al archivo descriptor con capacidad de lectura y escritura `    **Lo almacena  en formato `apent`**
![[Pasted image 20250311162557.png]]
`Cerrar el un descriptor de archivo ` pero esto no quiere decir que el archivo haya perdido su contenido
![[Pasted image 20250311162853.png]]   ![[Pasted image 20250311162935.png]]
`Crear copia de un descriptor (meter algo por alguna copia o la read siempre llegara al archivo)`

```bash
┌──(kali㉿kali)-[~/Desktop/practicando]         Creamos el archivo
└─$ exec 5<> data

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ ls
data
   
┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ whoami >&5                             metemos whoami al descriptor 5

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ cat data
kali
  
┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ exec 8>&5                            decirmos que todo lo que esta en el descriptor 5 tambien lo tenga el 8 asi creamos y copiamos a la vez
 
┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ cat data                      
kali

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ pwd >&5                              metemos el output de pwd al descriptor 5    pwd es para ver la ruta en la que estamos

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ cat data
kali
/home/kali/Desktop/practicando

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ who -q >&8                           metemos el output de who -q al descriptor 8

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ cat data
kali
/home/kali/Desktop/practicando
kali
# users=1

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ exec 5>&-                            cerramos el descriptor 5

┌──(kali㉿kali)-[~/Desktop/practicando]  venos que al eliminar el descriptor 5 no se elimina nada
└─$ cat data
kali
/home/kali/Desktop/practicando
kali
# users=1

┌──(kali㉿kali)-[~/Desktop/practicando]  prueba de que al haber cerrado el descriptor principal la copia actua como si fuera la original 
└─$ cat /etc/hosts >&8

┌──(kali㉿kali)-[~/Desktop/practicando]
	└─$ cat data          
kali
/home/kali/Desktop/practicando
kali
# users=1
127.0.0.1       localhost
127.0.1.1       kali
::1             localhost ip6-localhost ip6-loopback
ff02::1         ip6-allnodes
ff02::2         ip6-allrouters
```

### EJERCICIO

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ exec 5<> gato

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ echo $PATH >&5   

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ cat gato
/home/kali/.local/bin:/usr/local/sbin:/usr/sbin:/sbin:/usr/local/bin:/usr/bin:/bin:/usr/local/games:/usr/games:/home/kali/.dotnet/tools

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ exec 6>&5     

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ whoami >&6

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ cat gato
/home/kali/.local/bin:/usr/local/sbin:/usr/sbin:/sbin:/usr/local/bin:/usr/bin:/bin:/usr/local/games:/usr/games:/home/kali/.dotnet/tools
kali

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ exec 5>&-    

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ pwd >&6  

┌──(kali㉿kali)-[~/Desktop/practicando]
└─$ cat gato
/home/kali/.local/bin:/usr/local/sbin:/usr/sbin:/sbin:/usr/local/bin:/usr/bin:/bin:/usr/local/games:/usr/games:/home/kali/.dotnet/tools
kali
/home/kali/Desktop/practicando
