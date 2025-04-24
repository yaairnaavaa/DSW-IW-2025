# 💻 Comandos Git 

A continuacion se presentan 20 comandos de GIT:

1. git init: 
El comando git init crea un nuevo repositorio git o reinicia uno existente.

Ejemplo: git init

2. git clone
Para copiar un repositorio Git de una ubicacion a otra, utilizamos el comando git clone. Normalmente copia un repositorio existente desde los servidores remotos como GitHub a la maquina local.

Ejemplo: git clone <URL_COPIADA>

3. git status
Muestra el estado de los archivos del repositorio

Ejemplo: git status

4. git add
Añade los cambios al area de preparación. Esto indica a Git que el repositorio debe actualizar estos cambios una vez que el usuario ejectue el comando confirmar.

Ejemplo: git add .
         git add

5. git commit
Guarda los cambios que has realizado en el repositorio local. 

Ejemplo: git commit -m "mensaje"

6. git remote add
Crea una conexion entre tu repositorio local y el repositorio remoto.

Ejemplo: git remote add <nombre_repositorio> <url_repositorio>

7. git push
Sincroniza el repositorio remoto con el repositorio local.

Ejemplo: git push <repositorio_remoto> <nombre_rama> 
         git push ---all origin
         git push --force origin main

8. git pull
Recupera y fusiona los cambios del repositorio remoto con los del repositorio local.

Ejemplo: git pull origin feature-branch
         

9. git fetch
Permite revisar los cambios en el repositorio remoto antes de fusionarlos en el local. 

Ejemplo: git fetch origin

10. git branch
Lista, crea o elimina ramas.

Ejemplo: grit branch
         git branch "nombre_rama"
         grit branch -d "nombre_rama"

11. git checkout
Cambiar de rama o restaurar archivos a un estado anterior

Ejemplo: git checkout -b "nombre_rama"
         git checkout -- <nombre_archivo>
         git checkout <nombre_rama> -- <nombre_archivo>

12. git merge:
Funsiona ramas diferentes

Ejemplo: git merge <nueva-rama> 

13. git rebase
Reaplica los commits de una rama sobre otra, reescribiendo el historial de forma más lineal. Muy útil para mantener un historial más limpio.

Ejemplo: git rebase <rama>

14. git log
Muestra un historial completo de todos los commits realizados en el repositorio, incluyendo autor, fecha y mensaje.

Ejemplo: git log

15. git diff
Muestra las diferencias entre archivos o ramas. Es útil para ver qué cambió línea por línea.

Ejemplo: git diff <archivo>

16. git reset
evierte cambios en el área de staging o elimina commits del historial según el modo usado (--soft, --mixed, --hard).

Ejemplo: git reset --hard HEAD~1

17. git stash
Guarda temporalmente los cambios que aún no se han confirmado (committed), para poder trabajar en otra cosa sin perder el trabajo.

Ejemplo: git stash

18. git stash pop
Recupera los cambios guardados con git stash y los aplica nuevamente al proyecto.

Ejemplo: git stash pop

19. git clean
Elimina archivos sin seguimiento (no versionados) del proyecto, como archivos temporales o generados.

Ejemplo: git clean -f

20. git config
Establece opciones de configuración para Git como el nombre del usuario, correo, editor predeterminado, etc.

Ejemplo: git config --global user.name "nombre_usuario"