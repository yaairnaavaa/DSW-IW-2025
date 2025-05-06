## Sergio Michael Robles Zambrano
## 20400810 - 20 Comandos 

## Comando: git init
## Descripcion
Este comando se utiliza para inicializar un nuevo repositorio de Git. Crea un nuevo subdirectorio .git en tu directorio de trabajo actual. También creará una nueva rama llamada master.
## Ejemplo de casos de uso
git init
(Esto inicializará un repositorio de Git en tu directorio actual)

## Comando: git clone
## Descripcion
Este comando se utiliza para clonar un repositorio. Crea una copia de un repositorio remoto en tu máquina local.
## Ejemplo de casos de uso
git clone https://github.com/usuario/repositorio.git
(Esto clonará el repositorio en la URL determinada a tu máquina local)

## Comando: git add
## Descripcion
Este comando agrega un archivo al área de preparación como parte de un commit.
## Ejemplo de casos de uso
git add nombre_del_archivo
(Esto agregará el archivo llamado «nombre_del_archivo» al área de preparación)

## Comando: git commit
## Descripcion
Este comando se utiliza para guardar tus cambios en el repositorio local. Toma una instantánea de los cambios que has preparado usando git add.
## Ejemplo de casos de uso
git commit -m "Mensaje de confirmación"
(Esto confirmará tus cambios con un mensaje que describe lo que has cambiado)

## Comando: git status
## Descripcion
Este comando muestra el estado de los cambios como no rastreados, modificados o preparados
## Ejemplo de casos de uso
git status
(Esto mostrará el estado de tu directorio de trabajo)

## Comando: git pull
## Descripcion
Este comando obtiene cambios de un repositorio remoto y los fusiona en tu rama actual.
## Ejemplo de casos de uso
git pull origin master
(Esto obtendrá cambios de la rama master del repositorio remoto origin)

## Comando: git push
## Descripcion
Este comando envía tus cambios confirmados a un repositorio remoto.
## Ejemplo de casos de uso
git push origin master
(Esto enviará tus cambios confirmados a la rama master del repositorio remoto origin.)

## Comando: git branch
## Descripcion
Este comando enumera todas las ramas de tu repositorio.
## Ejemplo de casos de uso
git branch
(Esto enumerará todas las ramas de tu repositorio)

## Comando: git checkout
## Descripcion 
Este comando se utiliza para cambiar entre ramas en un repositorio de Git.
## Ejemplo de casos de uso
git checkout nombre_de_la_rama
(Esto cambiará a la rama llamada «nombre_de_la_rama«)

## Comando: git merge
## Descripcion
Este comando fusiona los cambios de una rama en otra.
## Ejemplo de casos de uso
(git merge nombre_de_la_rama)

## Comando: git diff
## Descripcion
Este comando muestra las diferencias de archivos que aún no están preparadas.
## Ejemplo de casos de uso
git diff
(Esto mostrará las diferencias no preparadas desde el último commit)

## Comando: git reset
## Descripcion
Este comando deshace la preparación del archivo, pero conserva su contenido.
## Ejemplo de casos de uso
git reset nombre_de_archivo
(Esto deshará la preparación del archivo llamado «nombre_de_archivo»)

## Comando: git rm
## Descripcion
Este comando elimina el archivo de tu directorio de trabajo y prepara la eliminación.
## Ejemplo de casos de uso
git rm nombre_de_archivo
(Esto eliminará el archivo llamado «nombre_de_archivo» y preparará la eliminación)

## Comando: git log
## Descripcion
Este comando muestra una lista de commits en una rama, incluidos los detalles correspondientes.
## Ejemplo de casos de uso
git log
(Esto mostrará una lista ordenada de los commits recientes)

## Comando: git fetch
## Descripcion
Este comando obtiene todos los objetos del repositorio remoto que no están presentes en el local.
## Ejemplo de casos de uso
git fetch origin
(Esto obtendrá todos los objetos del origen remoto que no existen en tu repositorio actual)

## Comando: git rebase
## Descripcion
Este comando se utiliza para aplicar los cambios realizados en la rama actual antes que en otra rama.
## Ejemplo de casos de uso
git rebase master
(Esto aplicará todos los cambios realizados en la rama actual por delante de la rama maestra.)

## Comando: git revert
## Descripcion
Este comando crea un nuevo commit que deshace los cambios realizados en un commit anterior.
## Ejemplo de casos de uso
git revert HEAD
(Esto creará un nuevo commit que deshace los cambios realizados en el último commit)

## Comando: git stash
## Descripcion
Este comando guarda temporalmente los cambios que no deseas confirmar de inmediato. Puedes aplicar los cambios más tarde.
## Ejemplo de casos de uso
git stash
(Esto guardará temporalmente todos los archivos modificados seguidos)

## Comando: git stash pop
## Descripcion
Este comando restaura los cambios guardados más recientemente.
## Ejemplo de casos de uso
git stash pop
(Esto aplicará los cambios guardados más recientemente y los eliminará de la lista de guardados)

## Comando: git cherry-pick
## Descripcion
Este comando aplica los cambios introducidos en algunos commits existentes.
## Ejemplo de casos de uso
git cherry-pick ID_commit
(Esto aplicará los cambios introducidos por el commit con el ID dado)