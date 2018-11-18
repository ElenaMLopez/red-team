# CAPITULO 1. TERMINAL

**apt-get install terminator**
Usar el software Terminator = nos permite dividir la terminal de una manera muy práctica

### MANEJO BASICO TERMINAL

**Ifconfig** = muestra los datos de red, ip, mascara, broadcast...

**pwd** = ruta donde nos encontramos

**cd “directorio”** = nos mueve a ese directorio

**cd ..** = nos mueve al directorio anterior

**ls** = nos muestra los archivos y directorios donde nos encontramos

**ls -all** = muestra más detalles de los archivos y directorios, como permisos, tamaño, fecha de creación, etc...

**ls -all *.txt** = filtraría los txt

**grep -i “filtro”** = nos muestra la línea con la palabra a filtrar

**echo “información que queramos introducir” > nombrearchivo.txt** = crea un archivo .txt con esa información

**cat** = para leer un fichero

**nano** = para editar un fichero

**rm** = borrar archivo

**mkdir “directorio”** = crear directorio

**history** = para ver todos los comandos que hemos usado 

**rm -R “directorio”** = elimina un directorio

**cp “archivo para copiar” “nombre del archivo copiado”** = copiar archivos



### GESTION DE PROCESOS, PERMISOS Y BUSQUEDAS

#### PROCESOS

**ps** = para ver los procesos que están corriendo en el sistema (entorno de usuario)
**ps -all** = todos los procesos 
**“nombre del CMD” &** = dejar el proceso en segundo plano
**kill -9 “PID”** = para matar un proceso, el -9 es para forzar el cierre del proceso
top = ver los procesos y su consumo
**killall -9 “proceso”** = para matar varios procesos 
**bg** = para ver lo que tenemos en background
**fg** = para para volver al proceso que está en el background
**Cntrol+C** = termina el programa **Cntrol+Z** = lo mata  Cntrol+D = lo deja tal cual (background)

#### PERMISOS

**r = read 4   w = write 2   x = execute 1**

  - Los archivos están formados por 9 bits 3 grupos de tres, ejemplo: -rwx rwx rwx = 777
  
  - El primer grupo de 3 pertenece a los permisos del usuario actual, el segundo al grupo, y el tercero a otros usuarios del sistema.

**sudo su** = nos convierte en usuarios root con sus privilegios
**chmod 777 “archivo”** = para darle todos los permisos 
**chmod +rwx “archivo”** = daría los permisos “r w x” a los 3 grupos usuario, grupo y otros usuarios (777)

#### BUSQUEDAS

**grep -r “búsqueda” /** = nos buscaría todo lo que contuviese la palabra desde el directorio raíz
**locate “palabra a buscar”** = busca en la terminal la palabra
**updatedb** = actualizar la db
**whereis “palabra a buscar”** = busca la ruta
