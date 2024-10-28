### Como reparar o recuperar el escritorio

Un domingo mientras estaba aburrido me compre el MK11 y cuando lo quiera abrir me salia un error del sonido, cuando intente arreglar ese error por accidente borre el escritorio. Asi que en este lugar te dire como recuperar o reparlo si te esta fallando ^^.

## Linux Terminal

![Modo Terminal Linux](https://www.solvetic.com/uploads/monthly_01_2018/tutorials-9832-0-07627600-1515415697.png)

lo primero si es que se te borro el escritorio lo mas probable es que se te halla colocado esta vista, y si no la manera de entrar es `Ctrl+Alt+F1` o `Ctrl+Alt+F7`, depende de tu distrubicion.

En ese lugar primero tienes que colocar tu nombre de usuario y despues tu contraseña y en orden ejecutar estas lineas:

```bash
sudo su
```
>Cambia al usuario root, otorgando permisos administrativos completos. Es importante tener cuidado al usar este comando, ya que cualquier acción realizada tendrá privilegios de superusuario.

```bash
dpkg –configure -a
```
>Reconfigura todos los paquetes que están desempaquetados pero no configurados. Es útil para resolver problemas de instalación de paquetes.

```bash
apt-get -f install
```
>Intenta corregir dependencias rotas. La opción `-f` significa "fix-broken" (arreglar roto).

```bash
apt-get update
apt-get dist-upgrade
```

```bash
apt-get install –reinstall ubuntu-desktop
```

>Este comando reinstala el paquete `ubuntu-desktop`, que es el metapaquete para el entorno de escritorio de Ubuntu. Es útil si el entorno de escritorio está dañado o faltan componentes.

Despues solo reinicias

```bash
reboot
```

Y listo!!!, ya deberia Haberse reparado. Suerte .,.