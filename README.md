# intro_terminal
## Introducción a Unix y la SHELL

### Resumen

Práctico para entender UNIX


### Introducción

Unix es el sistema operativo estándar para computoi científico. Algo similar sucede con Windows, pero en computadores de escritorio (PC).

Siguiendo esta comparativa, las similitudes entre ambos Sistemas Operativos son:

  - Se encargan de manejar el hardware por ud (redes, discos duros, procesador).

  - Proveen una interfaz para ejecutar aplicaciones y almacenar sus archivos.

  - Ambos poseen interfaces de escritorio que ofrecen casi las mismas prestaciones.


Por otra parte, Unix es seguro, estable y permite la ejecución de tareas con múltiples usuarios. Esto lo ha transformado en el sistema operativo de excelencia para computación de alto rendimiento (HPC: High Performance Computing). Se puede utilizar en diferentes tipos de hardware desde RaspberryPi, celulares y tablets (Android), notebook y PC hasta supercomputadores como Leftraru del [NLHPC](http://www.nlhpc.cl).

### Puesta a punto


Para facilitar este y los demás prácticos, he habilitado una de nuestras máquinas para la ejecución de tareas en este curso.

Además, en prácticos posteriores, algunos de los cálculos que realizaremos requeriran de un poder de cómputo moderado.  Por esto nos conectaremos a uno de los servidores de [Mathomics](http://www.mathomics.cl). 

Para esto necesitaremos una conexión a internet.

Si están en:

  - *Linux/MacOS*, puede utilizar [la terminal](https://help.ubuntu.com/kubuntu/desktopguide/es/terminals.html) (consola).

  - *Windows10* utilice el [Símbolo del sistema](https://es.wikipedia.org/wiki/S%C3%ADmbolo_del_sistema) (`cmd`).

  - Si están en *Windows* (anterior a *Windows 10*) deben instalar un programa llamado [Putty](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html).


### La Terminal

  - Es llamada *prompt*, *shell*, *línea de comandos*.

  - Antiguamente, era la única forma de interactuar con los computadores. 
  
  - La terminal es bastante agreste!.
 
  - Hablando en serio, es la interfaz que se utiliza para ejecutar comandos/programas o analizar los datos.

  - La mayoría de los programas que utilizamos a diario tienen una [GUI](https://es.wikipedia.org/wiki/Interfaz_gr%C3%A1fica_de_usuario)(Graphical User Interface). La mayoría de los programas más utilizados en Bioinformática no poseen una interfaz gráfica, esto principalmente porque los servidores donde se ejecutan los programas no tienen GUI, además de que requiere una etapa adiciónal de diseño y presupuesto.

  - Saber utilizar la terminal nos proveerá de una cantidad sustancial de ventajas en HPC.

### Protocolo SSH

Ahora, en la terminal, utilizaremos el protocolo [SSH](https://web.mit.edu/rhel-doc/4/RH-DOCS/rhel-rg-es-4/ch-ssh.html).

> :warning:  **NOTA**: De ahora en adelante, cada vez que vea `instrucción` se referira a un comando/programa a ejecutar, mientras que:

		esto será código a escribir en la terminal

> :warning: **NOTA**: En *Unix*, la terminal es *case sensitive*, es decir, escribir una `instrucción` es distinto a escribir  una `INSTRUCCIÓN` o `Instrucción` (*Windows* es diferente). Lo mismo pasa con los usuarios y los nombres de archivos. 

> :warning: **NOTA**: La mayoría de las veces, cuando tenga un problema al ejecutar una instrucción, se debe a errores tipográficos (*typos*). 
 
Una vez abierta la terminal (solo en *Win10*, *Linux*, *MacOS*), cada grupo debe escribir lo siguiente:

         ssh  usuario@servidor


> :warning: **NOTA**: Las credenciales se les entregaran en la pizarra.


Mediante el comando SSH podremos entrar al servidor de Mathomics. 

### Estructura de Directorios

En linux los directorios se organizan en una Jerarquía, es decir hay un directorio raíz y desde ese directorio se accede a sub-direcotrios.

Veremos la estructura de directorios de Unix en pizarra.

Dentro del servidor podemos ver donde estamos ubicados utilizando `pwd` ([print working directory](https://linux.die.net/man/1/pwd)). 

		pwd

Para saber el contenido del directorio donde estamos ubicados utilizamos `ls` ([list](https://linux.die.net/man/1/ls))


		ls

Si tenemos más de un directorio podemos ingresar a ese directorio con el comando `cd` ([change directory](http://linuxcommand.org/lc3_man_pages/cdh.html))

		cd ejemplo

### Revisar Archivos


Podemos mirar (Read Only) archivos con varios comandos como por ejemplo `more` ([man more](https://linux.die.net/man/1/more)):


		more sequencia1.fasta

También está el comando `less` ([man less](https://linux.die.net/man/1/less)):

		less secuencia1.fasta


Otro comando es `cat` ([man cat](https://linux.die.net/man/1/cat)):


		cat secuencia1.fasta

Hay diferencias?.

> :warning: **NOTA** `cat` es utilizado para concatenar archivos.


> :star: **HACK**:  Cuando quiere escribir un comando o buscar un directorio o escribir el nombre de un archivo, puede utilizar autocompletar con la tecla tab. [Link](https://i.ytimg.com/vi/KEkrWRHCDQU/hqdefault.jpg)


### Manual



