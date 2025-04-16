## ALDO REYMUNDO SAHAGUN GONZALEZ
## 20400820

`git init`  
Inicializa un nuevo repositorio Git en un directorio.  
`git init`  

`git clone`  
Copia un repositorio remoto a tu máquina local.  
`git clone https://github.com/usuario/repositorio.git`  

`git add`  
Añade cambios al área de staging (preparación).  
`git add archivo.txt`  

`git commit`  
Guarda los cambios del área de staging en el repositorio.  
`git commit -m "Mensaje descriptivo del cambio"`  

`git status`  
Muestra el estado de los archivos (modificados, staged, etc.).  
`git status`  

`git push`  
Envía los commits locales al repositorio remoto.  
`git push origin main`  

`git pull`  
Obtiene cambios del repositorio remoto y los fusiona con tu rama local.  
`git pull origin main`  

`git branch`  
Lista, crea o elimina ramas.  
`git branch nueva-rama`  

`git checkout`  
Cambia entre ramas o restaura archivos.  
`git checkout nueva-rama`  

`git merge`  
Fusiona una rama con la rama actual.  
`git merge nueva-rama`  

`git log`  
Muestra el historial de commits.  
`git log --oneline`  

`git diff`  
Muestra diferencias entre archivos o commits.  
`git diff archivo.txt`  

`git reset`  
Deshace cambios, moviendo el HEAD a un commit específico.  
`git reset --hard HEAD~1`  

`git remote`  
Gestiona conexiones con repositorios remotos.  
`git remote add origin https://github.com/usuario/repo.git`  

`git fetch`  
Descarga cambios del remoto pero no los fusiona.  
`git fetch origin`  

`git stash`  
Guarda cambios temporales sin hacer commit.  
`git stash pop`  

`git tag`  
Crea etiquetas para marcar versiones específicas.  
`git tag -a v1.0 -m "Versión 1.0"`  

`git rm`  
Elimina archivos del repositorio y del área de staging.  
`git rm archivo.txt`  

`git show`  
Muestra información detallada de un commit.  
`git show abc123`  

`git rebase`  
Reorganiza el historial de commits.  
`git rebase main`