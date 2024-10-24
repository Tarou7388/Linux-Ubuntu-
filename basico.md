## Navegación del sistema de archivos
# Comandos Básicos de Bash

## Navegación de directorios
- `ls`: Lista los archivos y directorios en el directorio actual.  
  **Ejemplo**: `ls`

- `cd [directorio]`: Cambia al directorio especificado.  
  **Ejemplo**: `cd /home/tarou`

- `pwd`: Muestra la ruta del directorio actual.  
  **Ejemplo**: `pwd`

## Manipulación de archivos y directorios
- `cp [origen] [destino]`: Copia archivos o directorios.  
  **Ejemplo**: `cp archivo.txt /backup/`

- `mv [origen] [destino]`: Mueve o renombra archivos o directorios.  
  **Ejemplo**: `mv archivo.txt nuevo_nombre.txt`

- `rm [archivo]`: Elimina archivos.  
  **Ejemplo**: `rm archivo.txt`

- `mkdir [directorio]`: Crea un nuevo directorio.  
  **Ejemplo**: `mkdir nuevo_directorio`

- `rmdir [directorio]`: Elimina un directorio vacío.  
  **Ejemplo**: `rmdir directorio_vacio`

## Información del sistema
- `uname -a`: Muestra información del sistema.  
  **Ejemplo**: `uname -a`

- `top`: Muestra los procesos en ejecución y el uso de recursos.  
  **Ejemplo**: `top`

- `df -h`: Muestra el uso del espacio en disco.  
  **Ejemplo**: `df -h`

- `free -h`: Muestra el uso de la memoria.  
  **Ejemplo**: `free -h`

## Gestión de paquetes
- `sudo apt update`: Actualiza la lista de paquetes disponibles.  
  **Ejemplo**: `sudo apt update`

- `sudo apt upgrade`: Actualiza los paquetes instalados.  
  **Ejemplo**: `sudo apt upgrade`

- `sudo apt install [paquete]`: Instala un nuevo paquete.  
  **Ejemplo**: `sudo apt install vim`

- `sudo apt remove [paquete]`: Elimina un paquete instalado.  
  **Ejemplo**: `sudo apt remove vim`

## Permisos y usuarios
- `chmod [permisos] [archivo]`: Cambia los permisos de un archivo.  
  **Ejemplo**: `chmod 755 script.sh`

- `chown [usuario]:[grupo] [archivo]`: Cambia el propietario de un archivo.  
  **Ejemplo**: `chown tarou:tarou archivo.txt`

- `sudo`: Ejecuta un comando con privilegios de superusuario.  
  **Ejemplo**: `sudo reboot`

## Red y conectividad
- `ping [host]`: Envía paquetes ICMP a un host para comprobar la conectividad.  
  **Ejemplo**: `ping google.com`

- `ifconfig`: Muestra la configuración de las interfaces de red.  
  **Ejemplo**: `ifconfig`

- `ssh [usuario]@[host]`: Conecta a un host remoto mediante SSH.  
  **Ejemplo**: `ssh tarou@192.168.1.1`

## Otros comandos útiles
- `grep [patrón] [archivo]`: Busca un patrón en un archivo.  
  **Ejemplo**: `grep "error" log.txt`

- `find [directorio] -name [nombre]`: Busca archivos por nombre en un directorio.  
  **Ejemplo**: `find /home/tarou -name "*.txt"`

- `tar -czvf [archivo.tar.gz] [directorio]`: Crea un archivo comprimido en formato tar.gz.  
  **Ejemplo**: `tar -czvf backup.tar.gz /home/tarou`

- `nano [archivo]`: Abre un editor de texto en la terminal.  
  **Ejemplo**: `nano archivo.txt`
