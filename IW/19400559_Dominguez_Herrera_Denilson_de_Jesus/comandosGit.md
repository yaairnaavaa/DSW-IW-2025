📄 Inicialización y configuración
git init
Inicializa un nuevo repositorio Git en el directorio actual.

git config --global user.name "Tu Nombre"
Configura el nombre del usuario globalmente.

git config --global user.email "tucorreo@example.com"
Configura el correo del usuario globalmente.

📁 Trabajando con archivos
git add archivo.txt
Agrega un archivo específico al área de staging.

git add .
Agrega todos los archivos modificados al área de staging.

git commit -m "Mensaje del commit"
Crea un commit con los cambios preparados.

git status
Muestra el estado de los archivos (modificados, en staging, no rastreados, etc.).

git rm archivo.txt
Elimina un archivo del repositorio y del sistema de archivos.

git mv archivo.txt nuevo_nombre.txt
Renombra o mueve un archivo.

🌿 Control de versiones
git log
Muestra el historial de commits.

git diff
Muestra los cambios entre el working directory y el área de staging.

git checkout nombre_rama
Cambia a otra rama.

git reset archivo.txt
Saca un archivo del área de staging.

git revert <hash_commit>
Crea un nuevo commit que revierte los cambios de uno anterior.

🌐 Trabajo con ramas
git branch
Muestra una lista de ramas.

git branch nueva_rama
Crea una nueva rama.

git merge nombre_rama
Fusiona otra rama con la rama actual.

git branch -d nombre_rama
Elimina una rama local.

☁️ Repositorios remotos
git clone url_del_repo
Clona un repositorio remoto.

git push origin nombre_rama
Envía los cambios de la rama al repositorio remoto.