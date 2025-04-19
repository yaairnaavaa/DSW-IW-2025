# Estos son los 20 comandos mas utilizados en git y su respctiva descripcion y ejemplo de uso.

# 1. Git init

    Descripcion: Inicializa un nuevo repositorio en el directorio actual.

    Ejemplo de uso : git init

# 2. Git clone

    Descripción: Clona un repositorio existente a tu máquina local.

    Ejemplo de uso: git clone https://github.com/usuario/repo.git

# 3. Git status

    Descripción: Muestra el estado del repositorio, incluyendo cambios y archivos en staging.

    Ejemplo de uso: git status

# 4. Git add

    Descripción: Añade archivos o cambios al área de staging.

    Ejemplo de uso: Para agregar un archivo especifico: git add archivo.txt
                    Para agregar todos los archivos: git add .

# 5. Git commit

    Descripción: Registra los cambios en el historial del repositorio con un mensaje descriptivo.

    Ejemplo de uso: git commit -m "Descripción del cambio realizado"

# 6. Git log

    Descripción: Muestra el historial de commits del repositorio.
    
    Ejemplo de uso: git log

# 7. Git push

    Descripción: Envía los cambios locales al repositorio remoto.

    Ejemplo de uso: git push origin main

# 8. Git pull

    Descripción: Recupera y fusiona cambios del repositorio remoto.
    
    Ejemplo de uso: git pull origin main

# 9. Git branch

    Descripción: Lista, crea o elimina ramas del repositorio.

    Ejemplo de uso: Para listar las ramas : git branch 
                    Para crear una rama: git branch nombre_rama
                    Para eliminar una rama: git branch -d nombre_rama
                    Para eliminar una rama que tiene cambios sin fusionar y quieres eliminarla de manera forzada: git branch -D nombre_rama

# 10. Git checkout

    Descripción: Cambia entre ramas o revisiones específicas.

    Ejemplo de uso: Para cambiar a una rama existente: git checkout nombre_rama
                    Para crear y cambiarte a una nueva rama al mismo tiempo: git checkout -b nombre_nueva_rama
                    Para revertir un archivo al estado de un commit anterior: git checkout commit_id -- nombre_archivo.txt
                    Para revertir el proyecto a un commit especifico: git checkout commit_id
                    Para recuperar un archivo eliminado: git checkout HEAD nombre_archivo.txt

# 11. Git merge

    Descripción: Fusiona cambios de una rama a otra.
    
    Ejemplo de uso: git merge nombre_rama

# 12. Git diff

    Descripción: Muestra las diferencias entre cambios no confirmados y el último commit.

    Ejemplo de uso: git diff

# 13. Git reset

    Descripción: Deshace cambios en el área de staging.

    Ejemplo de uso: Para quitar un archivo especifico del area de staging: git reset nombre_archivo.txt
                    Para eliminar todos los archivos del area de staging: git reset .
                    Se puede incliur la palabra HEAD para especificar que esto se hara en el ultimp commit realizado: git reset HEAD nombre_archivo.txt

# 14. Git rm

    Descripción: Elimina archivos del repositorio y del área de staging osea que los elimina fisicamente tambien.
    
    Ejemplo de uso: git rm archivo.txt

# 15. Git stash

    Descripción: Guarda cambios temporalmente para trabajar en otra cosa.

    Ejemplo de uso: git stash

# 16. Git tag

    Descripción: Crea una etiqueta para marcar un punto específico en el historial.
    
    Ejemplo de uso: git tag v1.0

# 17. Git fetch

    Descripción: Recupera datos del repositorio remoto pero no los fusiona.

    Ejemplo de uso: git fetch origin

# 18. Git remote

    Descripción: Administra las conexiones con repositorios remotos.

    Ejemplo de uso: git remote -v

# 19. Git rebase

    Descripción: Reaplica commits sobre un nuevo base branch.

    Ejemplo de uso: git rebase nombre-rama

# 20. Git mv

    Descripción: Renombra o mueve un archivo en el repositorio.

    Ejemplo de uso: git mv archivo-viejo.txt archivo-nuevo.txt
