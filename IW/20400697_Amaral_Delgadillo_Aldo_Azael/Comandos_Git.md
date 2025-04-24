# Comandos para GitHub - Aldo Azael Amaral Delgadillo

### - Comandos Básicos Git - 

| Num | `Comando` | Descripción de comando | Ejemplo de caso de uso |
|:---------|:--------:|:--------:|---------:|
| 1    | `git init`  | Inicializa un nuevo repositorio Git |Cuando vayamos a iniciar un nuevo proyecto utilizaremos este comando si queremos llevar un control de versiones|
| 2    | `git clone`   | Clona un repositorio remoto en tu máquina local  |git clone git@github.com:yaairnaavaa/DSW-IW-2025.git|
| 3    | `git add .`  | Agrega todos los archivos al área de preparación antes del commit   |Cuando no queramos agregar archivo por achivo utilizaremos este comando para agregarlos todos de golpe |
| 4    | `git status`  | Muestra el estado actual del repositorio, archivos modificados, y los que están listos para el commit  | git status|
| 5    | `git commit -m ""`  | Guarda los cambios en el historial del repositorio junto con un mensaje  | git commit -m "Texto que identifique por que se hizo el commit" |
| 6    | `git log --oneline`  | Permite ver los commits que se han hecho  | Cuando queramos ver las diferentes versiones de nuestro proyecto y que no abarcen tanto espacio|

### - Navegar entre versiones -
| Num | `Comando` | Descripción de comando | Ejemplo de caso de uso |
|:---------|:--------:|:--------:|---------:|
| 7    | `git checkout ""`  | Permite cambiar a otra rama del proyecto o a otra versión   | git checkout main - git checkout a1b2c3d |
| 8    | `git fetch`  | Descarga los cambios del repositorio remoto, pero no los fusiona | git fetch origin|
| 9    | `git reset --hard ""`  | Cambia el master al commit que le digamos y se eliminaran las versiones posteriores a esta, modifica nuestros archivos a esa versión | git reset --hard a1b2c3d|

### - Ramas -
| Num | `Comando` | Descripción de comando | Ejemplo de caso de uso |
|:---------|:--------:|:--------:|---------:|
| 10    | `git checkout -b ""`  | Creamos y nos movemos a otra rama  | git checkout -b "20400697" |
| 11    | `git branch`  | Nos muestra que ramas hay y en cual nos encontramos  | Cuando queramos ver las ramas del proyecto |
| 12	    | `git merge`  | Fusiona una rama con otra  | git merge 20400697|
| 13	    | `git push -u origin "rama"`  | Envía tus commits locales de una rama al repositorio remoto  | git push -u origin main|
| 14	    | `git pull origin "rama"`  | Trae y fusiona los cambios del repositorio remoto al local  | git pull origin main|

### - Eliminar -
| Num | `Comando` | Descripción de comando | Ejemplo de caso de uso |
|:---------|:--------:|:--------:|---------:|
| 15    | `rm ""`  | Elimina archivos del repositorio y del área de preparación| git rm archivo.txt|
| 16    | `rm -rf .git*`  | Se remueve git del proyecto | Cuando queramos eliminar git de nuestro proyecto|

### - Comandos Random -
| Num | `Comando` | Descripción de comando | Ejemplo de caso de uso |
|:---------|:--------:|:--------:|---------:|
| 17    | `git tag`  | Crea una etiqueta en un commit específico, útil para versiones| git tag v1.0|
| 18    | `git diff`  | Muestra las diferencias entre archivos o ramas| git diff archivo.txt|
| 19    | `git revert`  | Crea un nuevo commit que revierte los cambios de un commit anterior| git revert 1234abcd|
| 20    | `git show`  | Muestra detalles de un commit específico (autor, fecha, cambios)| git show a1b2c3d|