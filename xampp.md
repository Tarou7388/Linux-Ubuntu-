# Instalación de XAMPP en Linux y actualización de SQL

Cuando instalé XAMPP en Linux, me resultó algo fácil. Sin embargo, al intentar probar SQL, me salió un error que no me dejaba avanzar. El error era el siguiente:

> ERROR 1558 (HY000): Column count of mysql.proc is wrong. Expected 21, found 20. Created with MariaDB 100108, now running 100425. Please use mysql_upgrade to fix this error.


Esto se debe a que SQL no está actualizado (lo cual no entiendo por qué). A continuación, te explicaré cómo instalar XAMPP y actualizar SQL.

## Instalacion

Para instalarlo primero tenemos que decargar el archivo de instalacion del xampp para linux. [XAMPP install](https://www.apachefriends.org/es/download.html)

> [!NOTE]
> Recuerda siempre instalar la ultima version de este.

Despues solo ejecute lso comando de instalacion.

1. Ve a la carpeta de instalacion, en mi caso es Descargas asi que entrare alli

```bash
cd Descargas
```

2. Dale los permisos al instalador (el * es la version del xampp). Para no escribir todo solo coloca xampp y pulsa tab para autocompletar

```bash
chmod 755 xampp-linux-*-installer.run
```

3. ejecuta el instalador

```bash
sudo ./xampp-linux-*-installer.run
```
¡Listo ya lo instalaste!

## Abrir xampp

Primero que nada xampp no tiene un ejecutable en linux como Windows o macOS
para abrirlo se hace por la terminal

```bash
cd /opt/lampp
```
```bash
sudo ./manager-linux-x64.run
```
te recomiendo usarlo solo para cunado quieres hacer uno que otro cambio, pero si quieres ejecutarlo mejor usa el comando que te da el mismo xampp:

```bash
sudo /opt/lampp/lampp start
```
y para pararlo es:

```bash
sudo /opt/lampp/lampp stop
```

> [!NOTE]
> Te recomiendo ponerle un alias a estos comando para que no solo no tengas que entrar en el navegador a buscarlos, sino para no escribirlo a cada rato. Explico como hacer el alias en el archivo recomendaciones_personales.md

## Intalar extenciones de php

Para instalar extenciones solo tinenes que ejecutar este comando: 

```bash
sudo apt install php-gmp
```
pero primerp tienes que actualizar el apt, despues reinicias el apache

```bash
sudo systemctl restart apache2
```

[^1]: [XAMPP documentacion](https://www.apachefriends.org/es/faq_linux.html).
[^2]: pagina donde encontre la solucion al problema: [Aqui](https://dba.stackexchange.com/questions/322866/error-1558-hy000-column-count-of-mysql-proc-is-wrong-how-do-i-solve-this).