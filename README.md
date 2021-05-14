lista básica para git repositorios

for:
  git init( crear un repositorio  git en nuestro proyecto)
  rm -rf .git (elimina el repositorio git en nuestro proyecto)
  git status(muestra el estado de nuestro archivos, si han sido o no preparados(staging))
  git add file_name (adiciona los archivos al stagin area, uno a uno) 
  git add . (adiciona los archivos al stagin area, pero todos)
  git commit -m "commentary for the commit"( confirma los cambios realizados en nuestro proyecto)
  git remote add "repository" "url-git" ( git remote add origin "https://github.com/krlosjn/reposteria_uno.git")
  git push -u "repository" "branch" (git push origin master)
  git remote (muestra el nombre del repositorio)
  git fetch( trae los cambios de un repositorio remoto y los guarda en una carpeta oculta, generalmente se usa después un merge para mezclar esos cambios con la rama 
  que estamos trabajando)
  git checkout "branch_name"( me cambia de rama)
  git checkout -b "branch_name" (me permite crear una rama y pasarme automaticamente)
  git checkout -d "branch_name" (me permite eliminar una rama)
  git checkout --track "branch_name" (me permite crear una rama basada en una remota y mantener asociación con la rama remota)
  git merge "branch_name" (me permite fusionar una rama con otra, para esto nos ubicamos en la rama a la cual le añadiremos los cambios y luego 
  hacemos el merge para mezclar)
  git pull( me trae los cambios desde el repositorio remoto y luego.
  git rm -r --cached "file_name" ( los archivos seleccionados los elimina del area de preparación(staging))
  git stash ( me permite guardar cambios temporales para poder actualizar mi repositorio local desde el remoto) sirve mucho para cambios no confirmados
  y aún así queramos acutualizar nuestro workspace. 
  git stash pop( me permite después de hacer el fetch-merge o el pull traer los cambios que guarde antes )
  git reset me regresa el proyecto al commit indicado
  git reset --soft me regresa el proyecto al commit indicado manteniendo los cambios en el área de preparación 
  git reset --hard me regresa el proyecto al commit indicado eliminando los cambios realizados
  git push origin: "branch remoto"; (elimina rama remota);
