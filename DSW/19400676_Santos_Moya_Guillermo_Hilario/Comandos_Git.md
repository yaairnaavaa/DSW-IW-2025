COMANDSO MAS UTILIZADOS DE GIT

1. git init
Descripcion: Inicializa un nuevo repositorio Git en el directorio actual.
Ejemplo:
    git init

2. git clone
Descripcion: Clona un repositorio existente desde una URL remota.
Ejemplo:
    git clone https://github.com/usuario/repositorio.git

3. git add
Descripcion: Anade cambios al area de staging (preparacion).
Ejemplo:
    git add archivo.txt  # Anade un archivo especifico
    git add .            # Anade todos los archivos modificados

4. git commit
Descripcion: Guarda los cambios del area de staging en el historial del repositorio.
Ejemplo:
    git commit -m "Mensaje descriptivo del cambio"

5. git status
Descripcion: Muestra el estado de los archivos en el directorio de trabajo y el area de staging.
Ejemplo:
    git status

6. git pull
Descripcion: Obtiene los cambios del repositorio remoto y los fusiona con la rama actual.
Ejemplo:
    git pull origin main

7. git push
Descripcion: Envia los commits locales al repositorio remoto.
Ejemplo:
    git push origin main

8. git branch
Descripcion: Lista, crea o elimina ramas.
Ejemplo:
    git branch                  # Lista todas las ramas
    git branch nueva-rama       # Crea una nueva rama
    git branch -d rama-vieja    # Elimina una rama

9. git checkout
Descripcion: Cambia entre ramas o restaura archivos.
Ejemplo:
    git checkout rama-feature   # Cambia a la rama 'rama-feature'
    git checkout -- archivo.txt # Descarta cambios en un archivo

10. git merge
Descripcion: Fusiona una rama con la rama actual.
Ejemplo:
    git merge rama-feature

11. git log
Descripcion: Muestra el historial de commits.
Ejemplo:
    git log
    git log --oneline          # Muestra una version resumida

12. git diff
Descripcion: Muestra las diferencias entre archivos, commits o ramas.
Ejemplo:
    git diff                   # Muestra cambios no stageados
    git diff --staged          # Muestra cambios stageados

13. git reset
Descripcion: Deshace commits o cambios en el area de staging.
Ejemplo:
    git reset HEAD archivo.txt # Quita un archivo del staging
    git reset --hard HEAD~1    # Elimina el ultimo commit 

14. git remote
Descripcion: Gestiona conexiones a repositorios remotos.
Ejemplo:
    git remote -v              # Lista repositorios remotos
    git remote add origin URL  # Anade un repositorio remoto

15. git fetch
Descripcion: Descarga cambios del repositorio remoto sin fusionarlos.
Ejemplo:
    git fetch origin

16. git stash
Descripcion: Guarda cambios temporales sin hacer commit.
Ejemplo:
    git stash                  # Guarda cambios temporales
    git stash pop              # Recupera los cambios guardados

17. git tag
Descripcion: Crea, lista o elimina etiquetas (tags) para versiones.
Ejemplo:
    git tag v1.0.0             # Crea un tag
    git tag -l                 # Lista todos los tags

18. git rebase
Descripcion: Reorganiza el historial de commits.
Ejemplo:
    git rebase main

19. git cherry-pick
Descripcion: Aplica un commit especifico de otra rama.
Ejemplo:
    git cherry-pick abc1234    # Aplica el commit con hash abc1234

20. git config
Descripcion: Configura opciones de Git.
Ejemplo:
    git config --global user.name "Tu Nombre"
    git config --global user.email "tu@email.com"