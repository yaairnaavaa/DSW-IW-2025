**1. git init**  
   - Descripción: Inicializa un nuevo repositorio Git en el directorio actual.  
   - Ejemplo: `git init`  

**2. git clone [url]**  
   - Descripción: Clona un repositorio remoto en tu máquina local.  
   - Ejemplo: `git clone https://github.com/usuario/repo.git`  

**3. git add [archivo]**  
   - Descripción: Añade cambios específicos al área de preparación (staging).  
   - Ejemplo: `git add index.html`  

**4. git add .**  
   - Descripción: Añade todos los cambios (archivos nuevos/modificados) al staging.  
   - Ejemplo: `git add .`  

**5. git commit -m "mensaje"**  
   - Descripción: Guarda los cambios del staging en el repositorio con un mensaje descriptivo.  
   - Ejemplo: `git commit -m "Agregado el menú principal"`  

**6. git status**  
   - Descripción: Muestra el estado de los archivos (modificados, en staging, etc.).  
   - Ejemplo: `git status`  

**7. git push [remoto] [rama]**  
   - Descripción: Sube los commits locales al repositorio remoto.  
   - Ejemplo: `git push origin main`  

**8. git pull [remoto] [rama]**  
   - Descripción: Descarga cambios del repositorio remoto y los fusiona con tu rama local.  
   - Ejemplo: `git pull origin main`  

**9. git branch**  
   - Descripción: Lista todas las ramas locales. El asterisco (*) indica la rama actual.  
   - Ejemplo: `git branch`  

**10. git branch [nombre-rama]**  
    - Descripción: Crea una nueva rama.  
    - Ejemplo: `git branch feature-login`  

**11. git checkout [rama]**  
    - Descripción: Cambia a otra rama.  
    - Ejemplo: `git checkout feature-login`  

**12. git merge [rama]**  
    - Descripción: Fusiona una rama específica con la rama actual.  
    - Ejemplo: `git merge feature-login`  

**13. git log**  
    - Descripción: Muestra el historial de commits (ordenados del más reciente al más antiguo).  
    - Ejemplo: `git log`  

**14. git diff**  
    - Descripción: Muestra las diferencias entre archivos modificados y su última versión commitada.  
    - Ejemplo: `git diff`  

**15. git rm [archivo]**  
    - Descripción: Elimina un archivo del repositorio y del sistema de archivos.  
    - Ejemplo: `git rm archivo-obsoleto.txt`  

**16. git reset [archivo]**  
    - Descripción: Saca un archivo del área de staging (pero mantiene los cambios en el directorio).  
    - Ejemplo: `git reset archivo.html`  

**17. git remote -v**  
    - Descripción: Lista los repositorios remotos configurados.  
    - Ejemplo: `git remote -v`  

**18. git fetch [remoto]**  
    - Descripción: Descarga cambios del remoto pero no los fusiona con tu rama.  
    - Ejemplo: `git fetch origin`  

**19. git tag [nombre-tag]**  
    - Descripción: Crea un tag (etiqueta) para marcar un commit específico (útil para versiones).  
    - Ejemplo: `git tag v1.0.0`  

**20. git stash**  
    - Descripción: Guarda cambios temporales sin hacer commit (útil para cambiar de rama rápidamente).  
    - Ejemplo: `git stash`  