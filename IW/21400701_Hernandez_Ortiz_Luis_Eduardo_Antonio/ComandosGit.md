# Los 20 Comandos Más Usados de Git

1. **`git init`**
   - **Uso:** Inicializa un nuevo repositorio Git en un directorio.
   - **Ejemplo:** `git init`

2. **`git clone`**
   - **Uso:** Clona un repositorio remoto a tu máquina local.
   - **Ejemplo:** `git clone https://github.com/usuario/repositorio.git`

3. **`git status`**
   - **Uso:** Muestra el estado actual del repositorio (archivos modificados, no rastreados, etc.).
   - **Ejemplo:** `git status`

4. **`git add`**
   - **Uso:** Agrega cambios en archivos al área de preparación (staging area).
   - **Ejemplo:** `git add archivo.txt`

5. **`git commit`**
   - **Uso:** Guarda los cambios en el repositorio con un mensaje descriptivo.
   - **Ejemplo:** `git commit -m "Descripción del cambio"`

6. **`git push`**
   - **Uso:** Sube los cambios locales a un repositorio remoto.
   - **Ejemplo:** `git push origin main`

7. **`git pull`**
   - **Uso:** Trae y fusiona los cambios del repositorio remoto al repositorio local.
   - **Ejemplo:** `git pull origin main`

8. **`git fetch`**
   - **Uso:** Descarga los cambios del repositorio remoto sin fusionarlos automáticamente.
   - **Ejemplo:** `git fetch origin`

9. **`git log`**
   - **Uso:** Muestra el historial de commits del repositorio.
   - **Ejemplo:** `git log`

10. **`git diff`**
    - **Uso:** Muestra las diferencias entre los archivos modificados y los archivos en el repositorio.
    - **Ejemplo:** `git diff`

11. **`git branch`**
    - **Uso:** Muestra las ramas existentes en el repositorio o crea una nueva rama.
    - **Ejemplo:** `git branch nombre_rama`

12. **`git checkout`**
    - **Uso:** Cambia de una rama a otra o restaura archivos a un estado anterior.
    - **Ejemplo:** `git checkout nombre_rama`

13. **`git merge`**
    - **Uso:** Fusiona los cambios de una rama a la rama actual.
    - **Ejemplo:** `git merge nombre_rama`

14. **`git reset`**
    - **Uso:** Deshace cambios de commits previos (puede modificar el historial).
    - **Ejemplo:** `git reset --hard HEAD~1` (para deshacer el último commit)

15. **`git rm`**
    - **Uso:** Elimina archivos del repositorio.
    - **Ejemplo:** `git rm archivo.txt`

16. **`git stash`**
    - **Uso:** Guarda temporalmente los cambios no confirmados (útil cuando quieres cambiar de rama sin hacer commit).
    - **Ejemplo:** `git stash`

17. **`git tag`**
    - **Uso:** Marca puntos específicos en la historia de un repositorio (usualmente para versiones).
    - **Ejemplo:** `git tag v1.0`

18. **`git config`**
    - **Uso:** Configura opciones de Git (como el nombre de usuario y el correo electrónico).
    - **Ejemplo:** `git config --global user.name "Tu Nombre"`

19. **`git remote`**
    - **Uso:** Muestra o manipula los repositorios remotos (como agregar un remoto o cambiar la URL).
    - **Ejemplo:** `git remote add origin https://github.com/usuario/repositorio.git`

20. **`git revert`**
    - **Uso:** Crea un nuevo commit que deshace los cambios de un commit anterior (a diferencia de `reset`, mantiene el historial intacto).
    - **Ejemplo:** `git revert <id_commit>`