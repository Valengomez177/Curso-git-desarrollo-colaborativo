# Clase 02 - Git Desarrollo Colaborativo

## .gitkeep 
Es un archivo que me permite hacer un commit para guardar una carpeta que no es detectada por git cuando esta vacía.

## .gitignore
Es un archivo que nos permite ignorar archivos o carpetas completas que no quiero que se guarden dentro del repositorio.
Se escribe siempre en la raiz del proyecto.

## Marcar archivos que quiero que sean parte del próximo commit
Osea marcar archivos que estan en el working directory terminado y quiero llevarlos al área de confirmación para que sean parte del próximo commit.

```sh 
git add <nombre-archivo1> <nombre-archivo2>
git add <nombre-archivo>
git add README.md
```

## Ver el contenido de un commit hecho

```sh
git show <hash>
git show 321ad9c
```

## Guardar los cambios en el repositorio 

```sh 
git commit -m "Mensaje"
git commit # Se abre el editor para escribir el mensaje
git commit -a # Se hace un add de los archivos modificados, no se hace un add de los archivos untracked y se abre el editor para escribir el mensaje
git commit -am "Mensaje" # Se agregan los archivos modificados y no se abre el editor para escribir el mensaje
```

**NOTA**: Los mensajes idealmente pueden tener un máximo de 80 carácteres.

