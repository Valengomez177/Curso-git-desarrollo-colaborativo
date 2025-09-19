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
