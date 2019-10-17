# intro_terminal
## Introducción a Unix y la SHELL

### Resumen

Práctico para entender UNIX


### Introducción

Unix es el sistema operativo estándar para computoi científico. Algo similar sucede con Windows, pero en computadores de escritorio (PC).

Siguiendo esta comparativa, las similitudes entre ambos Sistemas Operativos es:

  - Se encargan de manejar el hardware por ud (redes, discos duros, procesador).

  - Proveen una interfaz para ejecutar aplicaciones y almacenar sus archivos.

  - Ambos poseen interfaces de escritorio que ofrecen casi las mismas prestaciones.


Por otra parte, Unix es seguro, estable y permite la ejecución de tareas con múltiples usuarios. Esto lo ha transformado en el sistema operativo de excelencia para computación de alto rendimiento (HPC: High Performance Computing). Se pueede utilizar en diferentes tipos de hardware desde RaspberryPi, celulares y tablets (Android), notebook y PC hasta supercomputadores como Leftraru del [NLHPC](http://www.nlhpc.cl).

## Trabajo preliminar:

Conectarse al servidor.

Para facilitar este y los demás prácticos, he habilitado una de nuestras máquinas para la ejecución de tareas en este curso.

Además, en prácticos posteriores, algunos de los cálculos que realizaremos requeriran de un poder de cómputo moderado.  Por esto nos conectaremos a uno de los servidores de [Mathomics](http://www.mathomics.cl). 

Para esto necesitaremos una conexión a internet.

Si están en:

  - `Linux/MacOS`, puede utilizar la terminal (consola).

  - `Windows10` utilice el [Símbolo del sistema](https://es.wikipedia.org/wiki/S%C3%ADmbolo_del_sistema) (`cmd`).

  - Si están en `Windows` (anterior a Windows 10) deben instalar un programa llamado [Putty](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html).

Ya, en la terminal, utilizaremos el protocolo [SSH](https://web.mit.edu/rhel-doc/4/RH-DOCS/rhel-rg-es-4/ch-ssh.html).
 
Una vez abierta la terminal (solo en Win10, Linux, MacOS), cada grupo debe escribir lo siguiente:

         ssh  usuario@servidor


> :warning: **NOTA**: Las credenciales se les entregaran en la pizarra. En el nombre de usuario y la contraseña, la `N` debe ser reemplazada por el número del grupo que fue asignado.

Mediante el comando SSH podremos entrar al servidor de Mathomics. 

Ya en el servidor podemos ver donde estamos ubicados utilizando el comando `pwd`.

> :warning:  **NOTA**: De ahora en adelante, cada vez que vea `instrucción` se referira a un comando de Unix, mientras que:

		esto será código a escribir en la terminal

