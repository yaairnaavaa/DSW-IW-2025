# Crear archivo llamado Comandos_Git.md (Investigar 20 comandos)

1. **Comando:** `git init`  
   **Descripción:** Iniciamos GIT en la carpeta donde está el proyecto  
   **Ejemplo de uso:**

   - Cuando ejecutas el comando, tu directorio actual se convierte en un repositorio Git, lo que te permite seguir sus cambios.

2. **Comando:** `git clone`  
   **Descripción:** Normalmente copia un repositorio existente, incluyendo registros y versiones, desde servidores remotos como GitHub.  
    **Ejemplo de uso:**

   - git clone <copied_URL>

3. **Comando:** `git status`  
   **Descripción:** El comando git status nos muestra detalles.  
   **Ejemplo de uso:**

   - Archivos modificados (archivos modificados pero no puestos en escena).
   - Archivos no rastreados (archivos que Git no está rastreando).

4. **Comando:** `Comando: Git add o Git add`  
   **Descripción:** El comando git add añade tus cambios al área de preparación. Indica a Git que el repositorio debe actualizar estos cambios una vez que el usuario ejecute el comando confirmar.  
   **Ejemplo de uso:**

   - git add . : escenifica los cambios realizados en todos los archivos.
   - git add : incluye sólo los cambios realizados en un archivo concreto del área de preparación.

5. **Comando:** `git commit`  
   **Descripción:** El comando git commit guarda los cambios que has realizado (o puesto en escena) en el repositorio local.  
   **Ejemplo de uso:**  
   git commit -m "commit_message"

6. **Comando:** `git push`  
   **Descripción:** El comando git push sincroniza tu repositorio remoto con el repositorio local. Una vez que ejecutes este comando, el repositorio remoto reflejará todos los cambios que hayas confirmado localmente.  
   **Ejemplo de uso:**

   - git push <remote> <branch>

7. **Comando:** `git pull`  
   **Descripción:** El comando git pull recupera y fusiona los cambios del repositorio remoto con los del repositorio local.  
   **Ejemplo de uso:**

   - git pull origin feature-branch

8. **Comando:** `git fetch`  
   **Descripción:** El comando git fetch te permite revisar los cambios en el repositorio remoto antes de fusionarlos en el local. Descarga los cambios y los actualíza en ramas de seguimiento remotas.  
   **Ejemplo de uso:**

   - git fetch origin

9. **Comando:** `git branch`  
   **Descripción:** El comando git branch lista, crea o elimina ramas. Una rama es otra versión de tu repositorio.  
   **Ejemplo de uso:**

   - git branch -a
   - git branch nombre_rama
   - git branch -d nombre_rama

10. **Comando:** `git checkout`  
    **Descripción:** El comando git checkout puede hacer dos cosas: cambiar entre ramas o restaurar archivos a un estado anterior.  
    **Ejemplo de uso:**

    - git checkout -b feature_branch
    - git checkout -- <file-name>

11. **Comando:** `git merge`  
    **Descripción:** Si has realizado algún trabajo en una nueva rama, puedes fusionarla con la rama principal utilizando git merge para implementar los cambios.  
    **Ejemplo de uso:**

    - git merge nombre_rama

12. **Comando:** `git rebase`  
    **Descripción:** git rebase es otra forma de integrar cambios entre ramas, pero funciona de forma distinta a git merge. Fusionar conserva el historial completo tanto de la rama principal como de la rama de características. Rebase, por otro lado, sobrescribe el historial de confirmaciones para hacerlo lineal y limpio.  
    **Ejemplo de uso:**

    - git checkout feature/login
    - git rebase main

13. **Comando:** `git log`  
    **Descripción:** El comando git log muestra todo el historial de confirmaciones de tu rama actual. Incluye cuatro campos clave: confirmación, autor, fecha y mensaje de confirmación.  
    **Ejemplo de uso:**

    - git log

14. **Comando:** `git diff`  
    **Descripción:** La página git diff muestra las diferencias entre varios estados de tu repositorio, ya sea comparando tu directorio actual con el área de preparación, el área de preparación con la última confirmación, o incluso dos archivos o ramas, lo que especifiques.  
    **Ejemplo de uso:**

    - git diff -

15. **Comando:** `git reset`  
    **Descripción:** El comando git reset te permite deshacer cambios restableciendo el HEAD actual a un estado anterior específico.Para mover el HEAD a un commit anterior, tienes tres variantes: "suave", "mixta" y "dura" para utilizarlas con el comando reiniciar.  
    **Ejemplo de uso:**

    - git reset --soft HEAD~1
    - git reset --mixed HEAD~1
    - git reset --hard HEAD~1

16. **Comando:** `git stash`  
    **Descripción:** Supongamos que quieres moverte a un estado anterior pero no quieres comprometer tu progreso actual; puedes utilizar git stash. Esto guarda temporalmente tus cambios no comprometidos y restablece tu directorio de trabajo al último estado comprometido.  
    **Ejemplo de uso:**

    - git stash

17. **Comando:** `git clean`  
    **Descripción:** El comando git clean borra los archivos sin seguimiento del repositorio Git.  
    **Ejemplo de uso:**

    - git clean

18. **Comando:** `git stash pop`  
    **Descripción:** Aplica los últimos cambios almacenados al directorio de trabajo.  
    **Ejemplo de uso:**

    - git stash pop

19. **Comando:** `git config`  
    **Descripción:** Configura las opciones de Git a nivel de sistema, global o local.  
    **Ejemplo de uso:**

    - git config --global user.name 'Your Name'

20. **Comando:** `git switch`  
    **Descripción:** Pasar de una rama a otra (preferible en versiones más recientes).  
    **Ejemplo de uso:**
    - git switch

# Referencias bibliográficas

- DataCamp. (4 de marzo de 2025). Los 20 mejores comandos Git con ejemplos: Guía práctica.  
  https://www.datacamp.com/es/blog/git-commands
