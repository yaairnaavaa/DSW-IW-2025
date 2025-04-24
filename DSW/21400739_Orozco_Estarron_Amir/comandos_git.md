1. git init
Descripción: Inicializa un nuevo repositorio Git.
Ejemplo: git init
Crea un repositorio Git vacío en el directorio actual.

2. git clone
Descripción: Clona un repositorio remoto en tu computadora.
Ejemplo: git clone https://github.com/usuario/repositorio.git
Descarga una copia del repositorio de GitHub en tu máquina local.

3. git status
Descripción: Muestra los archivos modificados, nuevos o eliminados.
Ejemplo: git status
Te dice qué archivos están listos para hacer commit y cuáles no.

4. git add
Descripción: Agrega archivos al área de preparación para ser confirmados.
Ejemplo: git add archivo.txt
Prepara archivo.txt para ser incluido en el próximo commit.

5. git commit
Descripción: Guarda los cambios preparados en el historial del repositorio.
Ejemplo: git commit -m "Agregué archivo de comandos"
Crea un commit con un mensaje que describe los cambios hechos.

6. git push
Descripción: Sube los commits locales al repositorio remoto.
Ejemplo: git push origin main
Envía los commits de la rama main al repositorio remoto llamado origin.

7. git pull
Descripción: Trae y fusiona los cambios desde el repositorio remoto.
Ejemplo: git pull origin main
Descarga y fusiona los últimos cambios de la rama main del repositorio remoto.

8. git fetch
Descripción: Descarga los cambios del repositorio remoto pero no los fusiona.
Ejemplo: git fetch origin
Trae los nuevos commits del repositorio remoto, sin afectar tu trabajo local.

9. git merge
Descripción: Combina ramas diferentes.
Ejemplo: git merge rama-feature
Une los cambios de rama-feature a tu rama actual.

10. git branch
Descripción: Crea, muestra o elimina ramas.
Ejemplo: git branch nueva-rama
Crea una nueva rama llamada nueva-rama sin cambiarte a ella.

11. git checkout
Descripción: Cambia entre ramas o versiones de archivos.
Ejemplo: git checkout main
Cambia tu rama actual a main.

12. git log
Descripción: Muestra el historial de commits.
Ejemplo: git log
Muestra todos los commits hechos en la rama actual.

13. git config
Descripción: Configura opciones de Git, como el nombre de usuario o correo.
Ejemplo: git config --global user.name "Amir"
Configura tu nombre de usuario global en Git como Amir.

14. git remote
Descripción: Muestra o administra las conexiones a repositorios remotos.
Ejemplo: git remote -v
Muestra las URLs de los repositorios remotos vinculados.

15. git diff
Descripción: Muestra los cambios entre versiones o ramas.
Ejemplo: git diff
Muestra las diferencias entre los archivos modificados y los últimos guardados.

16. git reset
Descripción: Deshace cambios en el área de staging o en los commits.
Ejemplo: git reset archivo.txt
Quita archivo.txt del área de preparación sin borrar el archivo.

17. git revert
Descripción: Revierte un commit sin borrar el historial.
Ejemplo: git revert 123abc
Crea un nuevo commit que deshace los cambios del commit con hash 123abc.

18. git rm
Descripción: Elimina archivos del proyecto y del área de preparación.
Ejemplo: git rm archivo.txt
Elimina archivo.txt del proyecto y lo marca para ser eliminado en el próximo commit.

19. git stash
Descripción: Guarda temporalmente los cambios sin hacer commit.
Ejemplo: git stash
Guarda tus cambios no confirmados para poder trabajar en otra cosa sin perderlos.

20. git tag
Descripción: Marca puntos específicos en la historia del repositorio, como versiones.
Ejemplo: git tag v1.0
Crea una etiqueta llamada v1.0 en el commit actual.