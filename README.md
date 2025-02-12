# Comandos Básicos de Git

## Inicialización y Eliminación de Repositorios
- `git init`: Crear un repositorio git en nuestro proyecto.
- `rm -rf .git`: Elimina el repositorio git en nuestro proyecto.

## Estado y Preparación de Archivos
- `git status`: Muestra el estado de nuestros archivos, si han sido o no preparados (staging).
- `git add file_name`: Adiciona los archivos al área de preparación (staging), uno a uno.
- `git add .`: Adiciona todos los archivos al área de preparación (staging).

## Confirmación de Cambios
- `git commit -m "commentary for the commit"`: Confirma los cambios realizados en nuestro proyecto.

## Manejo de Remotos
- `git remote add "repository" "url-git"`: Añade un repositorio remoto (e.g., `git remote add origin "https://github.com/krlosjn/reposteria_uno.git"`).
- `git push -u "repository" "branch"`: Empuja los cambios a un repositorio remoto (e.g., `git push origin master`).
- `git remote`: Muestra el nombre del repositorio remoto.
- `git fetch`: Trae los cambios de un repositorio remoto y los guarda en una carpeta oculta, generalmente se usa después un merge para mezclar esos cambios con la rama en la que estamos trabajando.

## Cambio de Ramas
- `git checkout "branch_name"`: Cambia de rama.
- `git checkout -b "branch_name"`: Crea una nueva rama y cambia a ella automáticamente.
- `git checkout -D "branch_name"`: Elimina una rama.
- `git checkout --track "branch_name"`: Crea una rama basada en una remota y mantiene la asociación con la rama remota.

## Fusión de Ramas
- `git merge "branch_name"`: Fusiona una rama con otra. Para esto, nos ubicamos en la rama a la cual le añadiremos los cambios y luego hacemos el merge para mezclar.
- ejemplo queremos mezclar develop en una feature, nos paramos en la feature y colocamos git merge develop

## Traer Cambios del Remoto
- `git pull`: Trae los cambios desde el repositorio remoto y los mezcla con nuestra rama actual.

## Eliminación de Archivos del Área de Preparación
- `git rm -r --cached "file_name"`: Elimina los archivos seleccionados del área de preparación (staging).

## Almacenamiento Temporal de Cambios
- `git stash`: Guarda cambios temporales para poder actualizar el repositorio local desde el remoto. Es útil para cambios no confirmados y aún así queremos actualizar nuestro workspace.
- `git stash pop`: Recupera los cambios guardados después de hacer `fetch-merge` o `pull`.

## Reinicio de Commits
- `git reset`: Regresa el proyecto al commit indicado.
- `git reset --soft  commit_code or branch_bame`: Regresa el proyecto al commit indicado manteniendo los cambios en el área de preparación.
- `git reset --hard commit_code`: Regresa el proyecto al commit indicado eliminando los cambios realizados.

## Eliminación de Ramas Remotas
- `git push origin: "branch remoto"`: Elimina una rama remota.
