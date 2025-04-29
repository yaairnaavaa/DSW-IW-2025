//Comandos en Git
1. git init
Descripción: Inicia git en la carpeta donde está el proyecto.
Ejemplo:
- cd miProyecto
- git init
2. git clone <url>
Descripción: Clona el repositorio de github desde la url indicada.
Ejemplo:
- git clone https://github.com/usuario/miProyecto.git
3. git add .
Descripción: Añade todos los archivos para el commit.
Ejemplo:
- git add .
4. git commit -m "Texto"
Descripción: Hace un commit con el texto que se quiera incluir.
Ejemplo:
- git commit -m "Agrego formulario de contacto"
5. git push origin main
Descripción: Sube al repositorio los cambios hechos localmente al main.
Ejemplo:
- git push origin main
6. git log
Descripción: Muestra los logs de los commits hechos.
- git log
Ejemplo:
7. git diff
Descripción: Muestra los cambios realizados a un archivo.
Ejemplo:
- git diff
8. git reset HEAD <archivo> 
Descripción: Saca un archivo del commit.
Ejemplo:
- git reset HEAD index.html
9. git remote add origin <url>
Descripción: Agrega un repositorio remoto.
Ejemplo:
- git remote add origin https://github.com/usuario/miProyecto.git
10. git remote rm <name/origin>
Descripción: Remueve un repositorio.
Ejemplo:
-git remote rm origin
11. git remote -v
Descripción: Muestra una lista de repositorios.
Ejemplo:
- git remote -v
12. git remote show origin
Descripción: Muestra los branches remotos.
Ejemplo:
- git remote show origin
13. git remote prune origin
Descripción: Limpia todos los branches eliminados.
Ejemplo:
- git remote prune origin
14. git branch <nombreBranch>
Descripción: Crea un branch con su respectivo nombre.
Ejemplo:
- git branch login-feature
15. git branch
Descripción: Lista los branches.
Ejemplo:
- git branch
16. git branch -d <nombreBranch>
Descripción: Elimina el branch uniéndolo a master.
Ejemplo:
- git branch -d login-feature
17. git tag
Descripción: Muestra una lista de los tags.
Ejemplo:
- git tag
18. git rebase
Descripción: Une el branch actual con el master.
Ejemplo:
- git checkout mi-feature
- git rebase main
19. git status 
Descripción: Lista un estado actual del repositorio con lista de archivos modificados o agregados.
Ejemplo:
- git status
20. git pull origin <nombreBranch>
Descripción: Busca los cambios nuevos y actualiza el repositorio.
Ejemplo:
- git pull origin main