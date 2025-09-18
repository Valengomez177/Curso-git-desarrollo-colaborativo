# Clase 01 - Git Desarrollo Colaborativo

## Página de Git
https://git-scm.com/

## Git con interfaz gráfica
>https://www.sourcetreeapp.com/
>https://www.gitkraken.com/
>https://desktop.github.com/download/

## Configuracion inicial
Está configuración se hace una sola vez. Y es para indicarle a git con que nombre y correo se van a firmar los commits creados
```sh
git config --global user.name "Maximiliano Principe"
git config --global user.email mlpeducacionit@gmail.com
```

## Verificar la configuración del usuario
```sh
git config --get-regexp user
```

## Listar configuraciones
```sh
git config --list
```

## Para editar las configuraciones
```sh
git config --global -e
```

## Para crear un repositorio de git
```sh 
git init
```
## En el caso de que no haya colocado en la instalación main

```sh
git config --global init-defaultBranch main
```

## Ver los commit generado (Timeline de commits)

```sh
git log # Versión larga
git log --oneline # Versión corta
```

## Estados de los archivos en un repositorio de GIT
> Untracked (Sin seguimiento) => archivos que no se agregaron al index/stage y por consecuente no se les da seguimiento.

> Staged => Archivos que fueron agregados al index/stage area y cuyos cambios van a ser incorporados al repositorio

> Unmodified => Archivos que se cuentran en en el respositorio y no fueron modificado (Con respecto al repositorio)

> Modified => Archivos que se encuentro en el repositorio pero difieren con lo que se encuentra actualmente en el directorio trabajo (Working directory)

## Areas posibles en las que pueden estar los archivos
> Working Directory (Directorio de trabajo) donde se van agregando y borrando archivos en el desarrollo

> Staging Area (Area de control de cambios) Se agregan los archivos para darle seguimiento y posteriormente sacarles una foto (commit)

> Local Repo (Area de validación de cambios, donde se registran las modificaciones realizadas) Donde van a estar todas las fotos (commit) que vaya sacando.

## Ayuda comandos
```sh
git <comando> --help
git status --help
git remote --help
git commit --help
```

## Para ver el estado de los archivos
```sh
git status
```

## Para pasar del WD al SA (Preparando los archivos para crear commits)
```sh
git add . # todos los archivos.
``` 

## Para pasar del SA al LR (Hacer un commits)
```sh
git commit -m "mensaje descriptivo de la tarea hecha"
```

## Para actualizar el repositorio remoto
```sh
git push
```