# git_course

## Class 2

Inicializar git en un proyecto
> git init

Ajustar main como nombre de la rama principal a usar por defecto
> git config --global init.defaultBranch main && git branch -m main

Listar los comandos de git
> git --help

Configuración de usuario por repo
> git config user.name "name-user"

Configuración de email por repo
> git config user.email "email-usuario"

Configuración **GLOBAL** de usuario por repo
> git config --global user.name "name-user"

Configuración **GLOBAL** de email por repo
> git config --global user.email "email-usuario"

**VALIDAR** la configuración
> git config --list


## Clase 3 - Git add | reset | commit

Agregar archivos al área de preparación (staging area)
> git add nombre-archivo.ext

Remover archivos del área de preparación (staging area)
> git reset nombre-archivo.ext

Commit de los archivos en el área de preparación (staging area)
> git commit -m "Mensaje del commit"

## Clase 4 - Git branch

Listar las ramas del repositorio
> git branch

Cambiar de rama o crear una nueva rama
> git switch nombre-rama

## Clase 5 -  Git reset | revert

Deshacer cambios hechos sin perder el historial de commits
> git revert [hash-commit-a-revertir]
#### Nos abre un editor para confirmar el commit de reversión. Recomendado agregar al mensaje el nombre del autor del commit que se revierte"

Deshacer cambios hechos eliminando solo los archivos modificados pero manteniendo el historial de commits
> git reset --soft [hash-commit-al-que-se-desea-volver]

Deshacer cambios hechos eliminando los archivos modificados y manteniendo el historial de commits, pero dejando los archivos modificados en el área de preparación (staging area)
> git reset --mixed [hash-commit-al-que-se-desea-volver]

Deshacer cambios hechos eliminando el historial de commits y los archivos modificados
> git reset --hard [hash-commit-al-que-se-desea-volver]
#### ¡CUIDADO! Este comando elimina los cambios hechos y no se pueden recuperar.

## Clase 6 - Git tag | Git checkout para gestion de versiones y revision.