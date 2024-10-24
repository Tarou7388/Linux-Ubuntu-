# Codigos extras que recomiendo

aqui unos comando que me facilitan la vida ^_^

## Alias para comandos

1. primero abres el el archivo `.bashtc`:
```bash
nano ~/.bashrc
```
O puedes usar otro editor como vim o gedit.

2. Agrega tu alias al final del archivo: Por ejemplo, para crear un alias que te permita usar `ll` en lugar de `ls -la`, añade la siguiente línea:

```bash
alias ll='ls -la'
```

3. Guarda los cambios y cierra el editor. (En nano, es `CTRL + O` despues pulsar enter). Despues cierralo con `CTRL + X`

4. carga los cambios en la terminal:

```bash
source ~/.bashrc
```

Y listo!!!


## Omitir la contraseña en la terminal

1. Lo primero es entrar en visudo con:

```bash
sudo visudo
```

2. Despues agregar al final del archivo este codigo:

```bash
<tu_nombre_user> ALL=(ALL) NOPASSWD: ALL
```
3. Guarda los cambios y cierra el editor. (En nano, es `CTRL + O` despues pulsar enter). Despues cierralo con `CTRL + X`

ahora ya no te va a pedor la contraseña cuando ejecutes cada comando