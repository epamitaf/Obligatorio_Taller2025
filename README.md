# Obligatorio Taller de Servidores Linux
## - Febrero 2025 -

Fatima Pereira (236544), Guido Soria (215451) 

---
### Configuraciones iniciales

Para poder realizar la tarea indicada fue necesario configurar tres servidores Linux. El primero, que tiene la funcionalidad de bastion con Centos Stream 9, habiendole instalado ansible, git y generado su clave publica. Otro de servidor web con Centros Stream 9 y uno con Ubuntu 24.04. Estos servidores proporcionan un espacio propicio para realizar las pruebas correspondientes al uso de git y ansible. 
En cada uno de los servidores se realizan las particiones correspondientes para boot, root, var y swap, asignandole un espacio determinado de memoria.

captura de las particiones

Estos servidores tienen dos interfaces de red, una interna y otra NAT para poder recibir instrucciones desde el bastion y poder conectarse a internet.  

En todos los servidores se crea el usuario sysadmin y se copia la clave publica del servidor bastion a los demas servidores para que puedan ser administrados por ssh.


> ### Creacion de repositorio y conexion a github

En primera instancia copiamos la clave publica del servidor bastion a nuestro usuario de github.

<div>
<p align:"center">
<img src="https://github.com/epamitaf/Obligatorio_Taller2025/blob/main/images/SSH1.png" alt="JuveYell" width="300px">
</p>
</div>

Creamos un repositorio publico en GitHub al que se le asigna el nombre Obligatorio_Taller2025 e inicializamos el archivo README.

En el servidor Centos que usamos de bastion clonamos el repositorio creado anteriormente con el comando `git clone git@github.com:epamitaf/Obligatorio_Taller2025.git` para poder tener nuestra staging area.

Luego de realizados los cambios permitenentes, ejecutamos el comando `git add .` agregarando los cambios realizados hasta ese momento. Una vez realizado esto, pasamos a ejecutar el comando `git commit -m "comentario"` para indicar los cambios realizados. Luego, para realizar la sicronizacion del repositorio local con el repositorio remoto, ejecutamos el comando `git push`.

> ### Pruebas comandos adhoc



<div>
<p align:"center">
<img src="https://github.com/epamitaf/Obligatorio_Taller2025/blob/main/images/1%20ansibleping.png" alt="JuveYell" width="500px">
</p>
</div>



<div>
<p align:"center">
<img src="https://github.com/epamitaf/Obligatorio_Taller2025/blob/main/images/2%20uptime.png" alt="JuveYell" width="500px">
</p>
</div>


<div>
<p align:"center">
<img src="https://github.com/epamitaf/Obligatorio_Taller2025/blob/main/images/3%20instalacion%20apache.png" alt="JuveYell" width="500px">
</p>
</div>



<div>
<p align:"center">
<img src="https://github.com/epamitaf/Obligatorio_Taller2025/blob/main/images/4%20espacio%20en%20disco%20ubuntu.png" alt="JuveYell" width="500px">
</p>
</div>

